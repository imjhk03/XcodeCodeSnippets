# Xcode Code Snippets

My personal collection of useful Xcode code snippets.

* [How to use](#how-to-use)
* [Collections](#collections)
  + [Collection view adapter](#collection-view-adapter)
  + [Mark](#mark)
  + [ViewModel Analytics](#viewmodel-analytics)
  + [Hack](#hack)
  + [Playground Page Title](#playground-page-title)
  + [Playground Page Next](#playground-page-next)

## How to use
1. Add any code snippet file to Xcode user's code snippets directory. Create one if doesn't exist.
```~/Library/Developer/Xcode/UserData/CodeSnippets```
2. Restart Xcode
3. Enjoy!

## Collections

### Collection view adapter
Creates a template for CollectionView, shortcut: ```collection view adapter```
```
// MARK: - UICollectionViewDataSource
extension <#AdapterName#>: UICollectionViewDataSource {
    func collectionView(_ collectionView: UICollectionView, numberOfItemsInSection section: Int) -> Int {
        <#code#>
    }
    
    func collectionView(_ collectionView: UICollectionView, cellForItemAt indexPath: IndexPath) -> UICollectionViewCell {
        <#code#>
    }
}

// MARK: - UICollectionViewDelegate
extension <#AdapterName#>: UICollectionViewDelegate {
    
}

// MARK: - UICollectionViewDelegateFlowLayout
extension <#AdapterName#>: UICollectionViewDelegateFlowLayout {
    
}
```

### Mark
Add Mark Line, shortcut: ```mark```
```
// MARK: - <#Name#>
```

### ViewModel Analytics
Create an extension of ViewModel for analytics. It has ```enum Event``` for various events, shortcut: ```viewmodel analytics```
```
// MARK: - Analytics
extension <#ViewModelName#> {
    enum Event {
        
    }
    
    func sendAnalyticsEvent(_ event: Event) {
        
    }
}
```

### Hack
Add comment describing hack code, shortcut: hack
```
// HACK: 
```

### Playground Page Title
Add Playground Page comment describing title, includes previous link, shortcut: title
```
/*:
 [< Previous](@previous)
 # - <#Title#>
*/
```

### Playground Page Next
Add Playground Page comment showing next page link, includes summary, shortcut: summary
```
/*:
 ## Summary
 1.
*/

//: [Next](@next)
```
