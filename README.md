
顶部滚动视图菜单 （常见的APP中顶部滚动菜单的选择， 使用UIScrollView进行封装，使用起来极其简单、实用、方便）

1、使用方法一：
    1、将项目中SGTopScrollMenu文件夹拖入工程
    2、导入#import "SGTopScrollMenu.h"头文件
    3、通过alloc、initWithFrame或者类方法topScrollMenuWithFrame去创建
    4、遵循SGTopScrollMenuDelegate协议的topScrollMenuDelegate方法（- (void)SGTopScrollMenu:(SGTopScrollMenu *)topScrollMenu didSelectTitleAtIndex:(NSInteger)index；）

2、使用方法二：（请参照Demo中的使用）

3、标题按钮是通过Label创建并在其上添加手势（UITapGestureRecognizer）

4、通过- (CGRect)boundingRectWithSize:(CGSize)size options:(NSStringDrawingOptions)options attributes:(nullable NSDictionary<NSString *, id> *)attributes context:(nullable NSStringDrawingContext *)context；方法，实现顶部标题按钮的自适应宽度
