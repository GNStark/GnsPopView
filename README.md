# GnsPopView
popView include tableView ，alertView and textView 

# popViewType
    tableViewPopView ,  //a tableView in popView;
    alertPopView ,     //a alertView in popView ,including title and buttom(s);
    textViewPopView    //a textView in popView ,including buttom; 

# GNSPopViewDelegate
- (void)textViewBtnClick:(NSString *)text;     // popViewType  == textViewPopView
- (void)alertBtnClick:(UIButton*)btn;          // popViewType  == alertPopView
- (void)popTableViewDidSelect :(NSIndexPath *)index; // popViewType == tableViewPopView

# init
- (instancetype)initWithFrame:(CGRect)frame WithType:(popViewType)popViewType ;

# showPoint 
you can let popView show from the point in screen;
@property (assign,nonatomic) CGPoint showPoint;
