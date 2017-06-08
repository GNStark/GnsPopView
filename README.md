# GnsPopView
popView include tableView ，alertView and textView 

# popViewType
    tableViewPopView ,  //a tableView in popView;
    alertPopView ,     //a alertView in popView ,including title and button(s);
    textViewPopView    //a textView in popView ,including button; 

# GNSPopViewDelegate
- (void)textViewBtnClick:(NSString *)text;     // popViewType  == textViewPopView
- (void)alertBtnClick:(UIButton*)btn;          // popViewType  == alertPopView
- (void)popTableViewDidSelect :(NSIndexPath *)index; // popViewType == tableViewPopView

# init
- (instancetype)initWithFrame:(CGRect)frame WithType:(popViewType)popViewType ;

# showPoint 
you can let popView show from the point in screen;
@property (assign,nonatomic) CGPoint showPoint;

# You can change property like shadowViewBackgroundColor 、button's title、count and more
