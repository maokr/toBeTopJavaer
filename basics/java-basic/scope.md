### 对于成员变量和方法的作用域，public,protected,private以及不写之间的区别。
- 类包括的变量和方法，变量和方法也自带访问属性
- 类是一座房子，钥匙就是对象，只有创建对象(拿到钥匙，才能进去访问)。
- public修饰的变量和方法，相当于不带锁的物品和房间。拿到对象后，就等于可以使用房间内的所有物品和房间。
- private修饰的变量和方法，相当于带锁的物品和带锁房间。那如何访问呢？这样的话，不能拿到对象.一下就访问了，可以让房间内的物品之间带上联系。比如有一间密室，方法是通过隔壁房间挖个洞去进入

成员变量：物品不是处在房间内(方法内)，一般拿到钥匙(对象)就能访问
局部变量：物品处在房间内(方法内)，首先拿到钥匙，再进入房间。且这个物品只能在房间使用，不能外带
如果成员变量和局部变量同名。则当你进入房间后，要对两者进行区分，this.成员变量名


- public :表明该成员变量或者方法是对所有类或者对象都是可见的,所有类或者对象都可以直接访问 
- private:表明该成员变量或者方法是私有的,只有当前类对其具有访问权限,除此之外其他类或者对象都没有访问权限.子类也没有访问权限. 
- protected:表明成员变量或者方法对类自身,与同在一个包中的其他类可见,其他包下的类不可访问,除非是他的子类 
- default:表明该成员变量或者方法只有自己和其位于同一个包的内可见,其他包内的类不能访问,即便是它的子类
