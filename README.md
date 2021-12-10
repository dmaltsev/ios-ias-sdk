# InAppStory

A library for embedding stories into an application with customization.

## Contents

* [Installation](https://github.com/inappstory/ios-sdk/tree/1.10.x#Installation)
	* [CocoaPods](https://github.com/inappstory/ios-sdk/tree/1.10.x#CocoaPods)
	* [Carthage](https://github.com/inappstory/ios-sdk/tree/1.10.x#Carthage)
	* [Swift Package Manager](https://github.com/inappstory/ios-sdk/tree/1.10.x#Swift-Package-Manager)
	* [Manual installation](https://github.com/inappstory/ios-sdk/tree/1.10.x#Manual-installation)
	* [Library import](https://github.com/inappstory/ios-sdk/tree/1.10.x#Library-import)
* [Migration](https://github.com/inappstory/ios-sdk/tree/1.10.x#migration)
* [InAppStory](https://github.com/inappstory/ios-sdk/tree/1.10.x#InAppStory)
	* [Initialization](https://github.com/inappstory/ios-sdk/tree/1.10.x#Initialization)
	* [Methods](https://github.com/inappstory/ios-sdk/tree/1.10.x#Methods)
	* [Parameters and properties](https://github.com/inappstory/ios-sdk/tree/1.10.x#Parameters-and-properties)
	* [Customization](https://github.com/inappstory/ios-sdk/tree/1.10.x#Customization)
* [StoryView](https://github.com/inappstory/ios-sdk/tree/1.10.x#StoryView)
	* [Initialization](https://github.com/inappstory/ios-sdk/tree/1.10.x#Initialization-1)
	* [Methods](https://github.com/inappstory/ios-sdk/tree/1.10.x#Methods-1)
	* [Parameters and properties](https://github.com/inappstory/ios-sdk/tree/1.10.x#Parameters-and-properties-1)
* [OnboardingStory](https://github.com/inappstory/ios-sdk/tree/1.10.x#OnboardingStory)
	* [Presentation](https://github.com/inappstory/ios-sdk/tree/1.10.x#Presentation)
* [SingleStory](https://github.com/inappstory/ios-sdk/tree/1.10.x#SingleStory)
	* [Presentation](https://github.com/inappstory/ios-sdk/tree/1.10.x#Presentation-1)
* [Protocols](https://github.com/inappstory/ios-sdk/tree/1.10.x#Protocols)
	* [InAppStoryDelegate](https://github.com/inappstory/ios-sdk/tree/1.10.x#InAppStoryDelegate)
	* [GoodsDelegateFlowLayout](https://github.com/inappstory/ios-sdk/tree/1.10.x#GoodsDelegateFlowLayout)
	* [StoryViewDelegate](https://github.com/inappstory/ios-sdk/tree/1.10.x#StoryViewDelegate)
	* [StoryViewDelegateFlowLayout](https://github.com/inappstory/ios-sdk/tree/1.10.x#StoryViewDelegateFlowLayout)
	* [OnboardingDelegate](https://github.com/inappstory/ios-sdk/tree/1.10.x#OnboardingDelegate)
	* [SingleStoryDelegate](https://github.com/inappstory/ios-sdk/tree/1.10.x#SingleStoryDelegate)
	* [PlaceholderProtocol](https://github.com/inappstory/ios-sdk/tree/1.10.x#PlaceholderProtocol)
	* [GamePlaceholderProtocol](https://github.com/inappstory/ios-sdk/tree/1.10.x#GamePlaceholderProtocol)
	* [StoryCellProtocol](https://github.com/inappstory/ios-sdk/tree/1.10.x#StoryCellProtocol)
	* [FavoriteCellProtocol](https://github.com/inappstory/ios-sdk/tree/1.10.x#FavoriteCellProtocol)
* [enum](https://github.com/inappstory/ios-sdk/tree/1.10.x#enum)
	* [ActionType](https://github.com/inappstory/ios-sdk/tree/1.10.x#ActionType)
	* [StoriesType](https://github.com/inappstory/ios-sdk/tree/1.10.x#StoriesType)
	* [ScrollStyle](https://github.com/inappstory/ios-sdk/tree/1.10.x#ScrollStyle)
	* [PresentationStyle](https://github.com/inappstory/ios-sdk/tree/1.10.x#PresentationStyle)
	* [ClosePosition](https://github.com/inappstory/ios-sdk/tree/1.10.x#ClosePosition)
	* [ActionType](https://github.com/inappstory/ios-sdk/tree/1.10.x#ActionType)
	* [GoodsFailure](https://github.com/inappstory/ios-sdk/tree/1.10.x#GoodsFailure)
* [Objects](https://github.com/inappstory/ios-sdk/tree/1.10.x#Objects)
	* [Settings](https://github.com/inappstory/ios-sdk/tree/1.10.x#Settings)
	* [WidgetStory](https://github.com/inappstory/ios-sdk/tree/1.10.x#WidgetStory)
	* [CustomGoodsView](https://github.com/inappstory/ios-sdk/tree/1.10.x#CustomGoodsView)
* [NotificationCenter](https://github.com/inappstory/ios-sdk/tree/1.10.x#NotificationCenter)
	* [Events](https://github.com/inappstory/ios-sdk/tree/1.10.x#Events)
	* [Errors](https://github.com/inappstory/ios-sdk/tree/1.10.x#Errors)
* [Samples](Samples/Samples.md)

## Installation

| InAppStory version | Build version | iOS version |
|--------------------|---------------|-------------|
| 1.10.6             | 1886          | >= 10.0     |

Version of the library can be obtained from the parameter `InAppStory.buildInfo`


### CocoaPods

[CocoaPods](https://cocoapods.org) is a dependency manager for Cocoa projects. For usage and installation instructions, visit their website. To integrate InAppStory into your Xcode project using CocoaPods, specify it in your `Podfile`:

```ruby
use_frameworks!
pod 'InAppStory', :git => 'https://github.com/inappstory/ios-sdk.git', :tag => '1.10.6'
```

### Carthage

[Carthage](https://github.com/Carthage/Carthage) is a decentralized dependency manager that builds your dependencies and provides you with binary frameworks. To integrate InAppStory into your Xcode project using Carthage, specify it in your `Cartfile`:

```ogdl
github "inappstory/ios-sdk" ~> 1.10.6
```

### Swift Package Manager

The [Swift Package Manager](https://swift.org/package-manager/) is a tool for automating the distribution of Swift code and is integrated into the `swift` compiler. It is in early development, but InAppStory does support its use on supported platforms.

Once you have your Swift package set up, adding InAppStory as a dependency is as easy as adding it to the `dependencies` value of your `Package.swift`.

```swift
dependencies: [
    .package(url: "https://github.com/inappstory/ios-sdk.git", .upToNextMajor(from: "1.10.6"))
]
```

### Manual installation

Download `InAppStorySDK.xcframework` from the repository. Connect in the project settings on the *General* tab.


### Library import

##### Objective-C

```objective-c
#import <InAppStorySDK/InAppStorySDK.h>
```

##### Swift

```swift
import InAppStorySDK
```
## Migration

* from InAppStorySDK - v 1.8.x -> [Migration guide to 1.9.0](https://github.com/inappstory/ios-sdk/blob/1.10.x/Migration-1.9.0.md)
* from InAppStorySDK - v 1.9.x -> [Migration guide to 1.10.0](https://github.com/inappstory/ios-sdk/blob/1.10.x/Migration-1.10.0.md)

## InAppStory

The main singleton class for managing data and customizing the display of lists and the reader.

### Initialization

Library Initialization is preferably carried out in `AppDelegate`: 

```swift
func application(_ application: UIApplication, didFinishLaunchingWithOptions launchOptions: [UIApplication.LaunchOptionsKey: Any]?) -> Bool 
{
	InAppStory.shared.initWith(serviceKey: <String>, testKey: <String>, settings: <Settings?>)
	return true
}
```

* `serviceKey` - service authorization key (\<*String*>); 
* `testKey ` - test authorization key in the service (\<*String*>);  
* `settings` - configuration object (*<[Settings?](https://github.com/inappstory/ios-sdk/tree/1.10.x#Settings)>* - *optional*).

>**Attention!**  
>If you pass *testKey*, then the library will display the stories only in the **"Moderation"** status.

### Methods

* `setTags(<Array<String>>)` - replace all tags;
* `addTags(<Array<String>>)` - adding tags;
* `removeTags(<Array<String>>)` - remove tags;
* `getWidgetStories(complete: (Array<WidgetStory>?) -> Void)` - getting a list of stories for a widget;
* `showOnboarding(from target: <UIViewController>, delegate: <OnboardingDelegate>, complete: @escaping () -> Void)` - show onboarding reader (**The method deprecated and will be removed in v1.11.x; Use showOnboardings**, [Migration guide](Migration.md));
* `showOnboardings(from target: <UIViewController>, delegate: <InAppStoryDelegate>, complete: @escaping () -> Void)` - show onboarding reader, also see *<[InAppStoryDelegate](https://github.com/inappstory/ios-sdk/tree/1.10.x#InAppStoryDelegate)>*
* `onboardingPresent(controller presentingViewController: <UIViewController>, with transitionStyle: <UIModalTransitionStyle>)` - serves for display of a custom controller over onboarding stories;
* `showSingleStory(with id: <String>, from target: <UIViewController>, delegate: <SingleStoryDelegate>, complete: @escaping () -> Void)` - show single reader (**The method deprecated and will be removed in v1.11.x; Use showSingle**, [Migration guide](Migration.md));
* `showSingle(with id: <String>, from target: <UIViewController>, delegate: <InAppStoryDelegate>, complete: @escaping () -> Void)` - show single reader, also see *<[InAppStoryDelegate](https://github.com/inappstory/ios-sdk/tree/1.10.x#InAppStoryDelegate)>*
* `singleStoryPresent(controller presentingViewController: <UIViewController>, with transitionStyle: <UIModalTransitionStyle>)` - serves for display of a custom controller over a single story;
* `clearCache` - clear all cache of library;

### Parameters and properties
* `favoritesCount` - the number of favorite stories a user has;
* `isLoggingEnabled` - displaying requests to the server in the console;
* `placeholders` - personalization substitution list *Dictionary\<String, String\>*;
* `widgetStories` - data for iOS widget.

### Customization

Customization of the appearance of the cells and the reader occurs through the singleton of the class `InAppStory.shared`:

#### List
* `coverQuality` - quality of cover images in cells *\<[Quality](https://github.com/inappstory/ios-sdk/tree/1.10.x#Quality)>*;
* `showCellTitle` - displaying story titles in a cell *\<Bool>*;
* `cellFont` - cell title font *\<UIFont>*;
* `cellBorderColor` - cell border color *\<UIColor>*;

#### Goods widget

* `goodsCellMainTextColor` - default goods item cell text color *\<UIColor>*;
* `goodsCellDiscountTextColor` - default goods item cell discount text color *\<UIColor>*;
* `goodCellTitleFont` - default goods item cell title font *\<UIFont>*;
* `goodCellSubtitleFont` - default goods item cell subtitle font *\<UIFont>*;
* `goodCellPriceFont` - default goods item cell price font *\<UIFont>*;
* `goodCellDiscountFont` - default goods item cell discount font *\<UIFont>*;
* `goodsCloseBackgroundColor` - close button background color *\<UIColor>*;
* `goodsSubstrateColor` - backround color under goods list *\<UIColor>*;
* `refreshGoodsImage` - images for refresh button *\<UIImage>*;
* `goodsCloseImage` - images for close button *\<UIImage>*;
* `goodCell` - custom cell, should implement the protocol *<[GoodsCellProtocol](https://github.com/inappstory/ios-sdk/tree/1.10.x#GoodsCellProtocol)>*;
* `goodsView` - custom goods view, should inherit from *<[CustomGoodsView](https://github.com/inappstory/ios-sdk/tree/1.10.x#CustomGoodsView)>*;
* `goodsDelegateFlowLayout` - should implement the protocol *<[GoodsDelegateFlowLayout](https://github.com/inappstory/ios-sdk/tree/1.10.x#GoodsDelegateFlowLayout)>*;

#### Reader
* `swipeToClose` - closing the reader by swipe *\<Bool>*;
* `overScrollToClose` - closing the reader when scrolling through the last story *\<Bool>*;
* `placeholderElementColor` - slide preloader color *\<UIColor>*;
* `placeholderBackgroundColor` - slide preloader background color *\<UIColor>*;
* `gamePlaceholderTint` - default game loader tint color *\<UIColor>*;
* `muted` - mute/unmute the sound in the story *\<Bool>*; (*[Details](Samples/Sound.md)*)
* `timerGradientEnable` - enable gradient shadow under timers in story *\<Bool>*;
* `likePanel` - displaying the bottom bar with likes (should be enabled in the console) *\<Bool>*;
* `favoritePanel` - displaying the bottom bar with favorites (should be enabled in the console) *\<Bool>*;
* `sharePanel` - displaying the bottom panel with sharing (should be enabled in the console) *\<Bool>*;
* `likeImage` - images for the like button *\<UIImage>*;
* `likeSelectedImage` - images for the selected like button *\<UIImage>*;
* `dislikeImage` - images for the dislike button *\<UIImage>*;
* `dislikeSelectedImage` - images for the selected dislike button *\<UIImage>*;
* `favoriteImage` - images for favorites button *\<UIImage>*;
* `favoriteSelectedImag` - images for selected favorites button *\<UIImage>*;
* `shareImage` - images for sharing button *\<UIImage>*;
* `shareSelectedImage` - images for selected sharing button *\<UIImage>*;
* `placeholderView` - custom loader, should implement the protocol *<[PlaceholderProtocol](https://github.com/inappstory/ios-sdk/tree/1.10.x#PlaceholderProtocol)>*;
* `gamePlaceholderView` - a custom game loader with progress, should implement the protocol *<[GamePlaceholderProtocol](https://github.com/inappstory/ios-sdk/tree/1.10.x#GamePlaceholderProtocol)>*;
* `closeButtonPosition` - the position of the close button relative to the timers *<[ClosePosition](https://github.com/inappstory/ios-sdk/tree/1.10.x#ClosePosition)>*;
* `scrollStyle` - animation style for slide transitions *<[ScrollStyle](https://github.com/inappstory/ios-sdk/tree/1.10.x#ScrollStyle)>*;
* `presentationStyle` - reader display style *<[PresentationStyle](https://github.com/inappstory/ios-sdk/tree/1.10.x#PresentationStyle)>*;

## StoryView

The main class for working with lists of stories.

### Initialization
---
**Remark**  
If the *settings* parameter was not specified for `InAppStory`, before initializing `StoryView`, it should be set:

```swift
InAppStory.shared.settings = Settings(userID: <String>, tags: <Array<String>?>)
```
---

If the parameter `favorite: <Bool?>` is equal true, the list will be displayed favorite stories.

```swift
var storyView: StoryView!
    
override func viewDidLoad() {
	super.viewDidLoad()
	
   	storyView = StoryView(frame: <CGRect>, favorite: <Bool?>)
	storyView.target = <UIViewController>
        
	view.addSubview(storyView)
        
	storyView.create()
}
```

### Methods

* `create` - running internal StoryView logic;
* `refresh` - refresh stories list;
* `clear` - clear cache of images;
* `closeStory(complete: () -> Void)` - closing the story reader with a closure, `complete` is called after the reader is closed; *(renamed to 'closeReader')*
* `closeReader(complete: () -> Void)` - closing any story reader that showinng with a closure, `complete` is called after the reader is closed;
* `present(controller presentingViewController: <UIViewController>, with transitionStyle: <UIModalTransitionStyle>)` - displaying a custom controller on top of the story reader.

### Parameters and properties

* `delegate` - should implement the protocol (**The property deprecated and will be removed in v1.11.x; Use storiesDelegate** [Migration guide](Migration.md));
* `storiesDelegate` - should implement the protocol *<[InAppStoryDelegate](https://github.com/inappstory/ios-sdk/tree/1.10.x#InAppStoryDelegate)>*;
* `deleagateFlowLayout` - should implement the protocol *<[StoryViewDelegateFlowLayout](https://github.com/inappstory/ios-sdk/tree/1.10.x#StoryViewDelegateFlowLayout)>*;
* `tags` - list of tags for content filtering *\<Array\<String>>*;
* `target` - controller for reader display *\<UIViewController>*;
* `isContent` - there is any content in the list of stories *\<Bool>*;
* `storyCell` - custom cell, should implement the protocol *<[StoryCellProtocol!](https://github.com/inappstory/ios-sdk/tree/1.10.x#StoryCellProtocol)>*;
* `favoriteCell` - custom favorites cell, should implement the protocol *<[FavoriteCellProtocol!](https://github.com/inappstory/ios-sdk/tree/1.10.x#FavoriteCellProtocol)>*;

## OnboardingStory

Onboarding is used to display stories not present in the main list.

### Presentation
---
**Remark**  
If the *settings* parameter was not specified for `InAppStory`, before showing onboarding, it should be set:

```swift
InAppStory.shared.settings = Settings(userID: <String>, tags: <Array<String>?>)
```
---

To display onboarding, you need call the `showOnboardings` method of the singleton class `InAppStory.shared`:

```swift
InAppStory.shared.showOnboardings(from target: <UIViewController>, delegate: <InAppStoryDelegate>, complete: <()->Void>)
```

To close the reader of onboarding, call `closeReader(complete: () -> Void)`. This may be necessary, such as when handling open the link by push a button in story. `complete` called after closing the reader.

## SingleStory

Used to display stories by their id or slug.

### Presentation
---
**Remark**  
If the *settings* parameter was not specified for `InAppStory`, before showing single story, it should be set:

```swift
InAppStory.shared.settings = Settings(userID: <String>, tags: <Array<String>?>)
```
---

To display single story, you need call the `showSingle` method of the singleton class `InAppStory.shared`:

```swift
InAppStory.shared.showSingle(from target: <UIViewController>, with id: <String>, delegate: <InAppStoryDelegate>, complete: <()->Void>)
```

To close the reader of single story, call `closeReader(complete: () -> Void)`. This may be necessary, such as when handling open the link by push a button in story. `complete` called after closing the reader.

## Protocols

### InAppStoryDelegate
* `storiesDidUpdated(isContent: <Bool>, from storyType: <StoriesType>, storyView: <StoryView>?)` - called after the contents are updated for sories type *<[StoriesType](https://github.com/inappstory/ios-sdk/tree/1.10.x#StoriesType)>*;
* `storyReader(actionWith target: <String>, for type: <ActionType>, from storyType: <StoriesType>, storyView: <StoryView>?)` - called after a link is received from stories with the interaction type *<[ActionType](https://github.com/inappstory/ios-sdk/tree/1.10.x#ActionType)>* and *<[StoriesType](https://github.com/inappstory/ios-sdk/tree/1.10.x#StoriesType)>*;
* `storyReaderWillShow(with storyType: <StoriesType>, storyView: <StoryView>?)` - called before the reader will show *(optional)*;
* `storyReaderDidClose(with storyType: <StoriesType>, storyView: <StoryView>?)` - called after closing the story reader *(optional)*;
* `favoriteCellDidSelect()` - called when the favorite cell has been selected *(optional)*;
* `getGoodsObject(with skus: <Array<String>>, complete: <GoodsComplete>)` - get goods items from parent app with closure, *<[GoodsComplete](https://github.com/inappstory/ios-sdk/tree/1.10.x#GoodsComplete)>*;
* `goodItemSelected(_ item: <Any>, with storyType: <StoriesType>, storyView: <StoryView>?)` - selected goods item in widget, with object sended in `getGoodsObject(...)`

### GoodsDelegateFlowLayout

Methods of delegate, like in UICollectionViewDelegateFlowLayout

* `sizeForItemAt() -> <CGSize>` - returns the cell size for the list;
* `insetForSection() -> <UIEdgeInsets>` - returns padding from the edges of the list for cells;
* `minimumLineSpacingForSection() -> <CGFloat>` - returns the vertical padding between cells in a list;

### StoryViewDelegate

* `storyViewUpdated(storyView: <StoryView>, widgetStories: Array<WidgetStory>?)` - called after the contents of the list are updated;
* `storyView(_ storyView: <StoryView>, actionWith type: <ActionType>, for target: <String>)
` - called after a link is received from stories with the interaction type *<[ActionType](https://github.com/inappstory/ios-sdk/tree/1.10.x#ActionType)>*;
* `storyReaderWillShow()` - called before the reader will show;
* `storyReaderDidClose()` - called after closing the story reader;
* `favoriteCellDidSelect()` - called when the favorite cell has been selected;

> **Pay attention!**  
> StoryViewDelegate deprecated and will be removed in v1.11.x; please migrate to a InAppStoryDelegate. [Migration guide](Migration.md)

### StoryViewDelegateFlowLayout

Methods of delegate, like in UICollectionViewDelegateFlowLayout

* `sizeForItemAt() -> <CGSize>` - returns the cell size for the list;
* `insetForSection() -> <UIEdgeInsets>` - returns padding from the edges of the list for cells;
* `minimumLineSpacingForSection() -> <CGFloat>` - returns the vertical padding between cells in a list;
* `minimumInteritemSpacingForSection() -> <CGFloat>` - returns horizontal padding between cells in a list;

### OnboardingDelegate

* `onboardingUpdated(isContent: <Bool>)` - called after the contents of the list are updated;
* `onboardingReader(actionWith target: <String>, for type: <ActionType>)` - called after a link is received from stories with the interaction type *<[ActionType](https://github.com/inappstory/ios-sdk/tree/1.10.x#ActionType)>*;
* `onboardingReaderWillShow()` - called before the reader will show;
* `onboardingReaderDidClose()` - called after closing the story reader;

> **Pay attention!**  
> OnboardingDelegate deprecated and will be removed in v1.11.x; please migrate to a InAppStoryDelegate. [Migration guide](Migration.md)

### SingleStoryDelegate

* `singleStoryUpdated(isContent: <Bool>)` - called after a single story is received;
* `singleStory(actionWith target: <String>, for type: <ActionType>)` - called after a link is received from stories with the interaction type *<[ActionType](https://github.com/inappstory/ios-sdk/tree/1.10.x#ActionType)>*;
* `singleStoryReaderWillShow()` - called before the reader will show;
* `singleStoryReaderDidClose()` - called after closing the story reader;

> **Pay attention!**  
> SingleStoryDelegate deprecated and will be removed in v1.11.x; please migrate to a InAppStoryDelegate. [Migration guide](Migration.md)

### PlaceholderProtocol  

* `isAnimate: <Bool> { get }` - returns the state of the animation
* `start` - start animation
* `stop` - stop animation

### GamePlaceholderProtocol  

* `func setProgress(progress: Double)` - setting the progress value (0.0 - 1.0)

### StoryCellProtocol

* `reuseIdentifier: <String> { get }` - returns cell reuse identifier;
* `nib: <UINib?> { get }` - returns the nib of the cell's visual representation; 
* `setTitle(_ text: <String>)` - story title;
* `setImageURL(_ url: <URL>)` - image url for cover;
* `setVideoURL(_ url: <URL>)` - video url for animated cover;
* `setOpened(_ value: <Bool>)` - set new state if story is opened;
* `setHighlight(_ value: <Bool>)` - set new state if story cell if highlighted;
* `setBackgroundColor(_ color: <UIColor>)` - background color of cell;
* `setTitleColor(_ color: <UIColor>)` - title color of cell;
* `setSound(_ value: Bool)` - does the story have sound;

### GoodsCellProtocol

* `reuseIdentifier: <String> { get }` - returns cell reuse identifier;
* `nib: <UINib?> { get }` - returns the nib of the cell's visual representation; 
* `setGoodObject(_ object: <Any>!)` - object that comes from `getGoodsObject(...)`;

### FavoriteCellProtocol

* `reuseIdentifier: <String> { get }` - returns cell reuse identifier;
* `nib: <UINib?> { get }` - returns the nib of the cell's visual representation;  

* `favoritesCount: Int { get set }` - total count of stories in favorites;
* `setHighlight(_ value: <Bool>)` - set new state if story cell if highlighted;
* `setImages(_ urls: <Array<URL?>>)` - a list of addresses of the first four images stories in favorites;
* `setImagesColors(_ colors: <Array<UIColor?>>)` - a list of background colors of the first four stories in favorites;
* `setBackgroundColor(_ color: <UIColor>)` - main background color of a cell;

## Closure

### GoodsComplete

Closure for contine `getGoodsObject(...)` method in *InAppStoryDelegate* - `(Result<Array<Any>, GoodsFailure>) -> Void`

## enum

### ScrollStyle

Story transition animation style in reader:  

* `.flat` - usual, one after another, like UIScrollView;
* `.cover` - covered with next slide;
* `.cube` - in the form of a 3D cube;


### PresentationStyle

Reader display animation style:

* `.crossDissolve` - showing reader from transparency;
* `.modal` - modal reader display;
* `.zoom` - display reader from list's cell;

### ClosePosition

Position of the close button on the card in the reader:

* `.left` - to the left of the timers;
* `.right` - to the right of the timers;
* `.bottomLeft` - on the left under the timers;
* `.bottomRight` - on the right under the timers;

### ActionType

The action by which the link was obtained:

* `.button` - push the button;
* `.swipe` - swipe up slide;
* `.game` - link from Game.

### StoriesType

The action by which the link was obtained:

* `.list` - type for StoryView;
* `.single` - type for single story reader;
* `.onboarding` - type for onboarding story reader.

### Quality

Quality of cover images in cells

* `medium`;
* `high`.

### GoodsFailure

Failure that return in `Result` from `getGoodsObject(...)` closure

* `refresh` - show refresh button in the *GoodsView*;
* `close` - close *GoodsView*.

## Objects

### Settings

#### Parameters

* `userID` - unique user identifier *\<String>*;
* `tags` - list of tags for content filtering *\<Array\<String>>*;

### WidgetStory

#### Parameters

* `id` - unique identifier of story *\<String>*;
* `title` - story title *\<String>*;
* `image` - link to cover image *\<String>*;
* `color` - background color of the story in HEX format *\<String>*;

### CustomGoodsView

To create your own goods widget, you need to inherit from CustomGoodsView.

* `setSKUItems(_ items: Array<String>)` - set SKUs of goods from InAppStory reader;
* `setReaderFrame(_ frame: CGRect)` - set StoryReader frame;
* `final close()` - needs call from *superclass*, for close widget;
* `final goodsItemClick(with sku: <String>)` - send statistic in SDK;

## NotificationCenter

### Events

Standard fields `userInfo`: `id`, `title`,` tags`, `slidesCount`. The exception is `StoriesLoaded`

* `StoriesLoaded` - the list of stories has loaded, `StoryView` is ready to work (fires every time the list is loaded, and also on refresh). In `userInfo` only field `count` - stories count;
* `ClickOnStory` - click on story in the list with additional parameters:
    * place where the click came from (`list` or `favorite`);
* `ShowStory` - display of the story reader with additional parameters:
    * `source` - place where the showing came from (`direct`, `onboarding`, `list` or `favorite`);
* `CloseStory` - closing story with additional parameters:
    * `index` - index of the slide from which the closure occurred,
    * `action` - closing action (`swipe`, `click`, `auto` or `custom`),
    * `source` - place where the closing came from (`direct`, `onboarding`, `list` or `favorite`);
* `ClickOnButton` - click on the button in the story with additional parameters:
    * `index` - index of the slide from which the get link,
    * `link` - string link;
* `ShowSlide` - show slide with additional parameters:
    * `index` - index of the slide that now show;
* `LikeStory` - story like with additional parameters:
    * `index` - index of the slide which "like" pressed,
    * `value` - value of "like" position (`true` - is like, `false` - isn't like);
* `DislikeStory` - story dislike with additional parameters:
    * `index` - index of the slide which "dislike" pressed,
    * `value` - value of "dislike" position (`true` - is dislike, `false` - isn't dislike);
* `FavoriteStory` - adding story to favorites with additional parameters:
    * `index` - index of the slide which "favorite" pressed,
    * `value` - value of "favorite" position (`true` - is favorite, `false` - isn't favorite);
* `ClickOnShareStory` - pushing the share button with additional parameters:
    * `index` - index of the slide which "share" pressed;
* `StartGame` - opening the reader with the game with additional parameters:
    * `index` - index of the slide which game start;
* `CloseGame` - closing the reader with the game with additional parameters:
    * `index` - index of the slide which game closed;
* `FinishGame` - closing the game at the end with additional parameters:
    * `index` - index of the slide which game finished,
    * `result<Dictionary<String, Any>?>` - game end results;

### Errors

In error notifications, `userInfo` also comes in the form of a dictionary `["errorMessage": <Error_message_string>]`

* `SessionFailure` - session error;
* `StoryFailure` - error in story;
* `CurrentStoryFailure` - error when loading full story information;
* `NetworkFailure` - network error (no internet);
