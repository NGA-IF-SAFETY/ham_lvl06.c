#I)HÀM
1.*CÁC KHÁI NIỆM*  
**-Chương Trình**:    
+Một chương trình C bao gồm một hoặc nhiều hàm      
+Hàm main() là thành phần bắt buộc của chương trình   
+Chương trình bắt đầu thực hiện từ câu lệnh đầu tiên của hàm main( ) cho đến khi gặp dấu } cuối cùng của hàm này    
**-Hàm**:   
+Là một đoạn chương trình độc lập thực hiện trọn vẹn một công việc rồi trả về một giá trị cho chương trình đã gọi nó.  
+Đặc điểm:    
            Là một đơn vị độc lập của chương trình  
            Không cho phép xây dựng một hàm bên trong một hàm khác  
2.**Xác định các thành phần của hàm**    
*Các thành phần của hàm bao gồm:*   
-Nguyên mẫu của hàm     
-Kiểu giá trị của hàm    
-Tên hàm   
-Các tham số của hàm   
-Nội dung cua hàm    
###a)nguyên mẫu hàm    
`<kiểu dl của hàm> <tên hàm(ds các tham số)>;`  
-Có thể có hoặc không khai báo nguyên mẫu của hàm  
-Tất cả nguyên mẫu của các hàm có trong chương trình nên đặt trước hàm main()   
###b)kiểu giá trị của hàm    
-Được xác định dựa vào mục đích của hàm   
-Nếu các hàm không trả về giá trị ta phải khai báo kiểu void    
###c) Tên hàm  
-Ðặt theo qui định đối với danh định   
-Tên hàm trong nguyên mẫu và khi khai báo phải giống nhau  
###d) Tham số của hàm : 
-*Phân loại theo cách sử dụng*  
-*Phân loại theo công dụng*  
###e)Nội dung của hàm   

                ` <Kiểu_trả_về>  <tên_hàm> `( [khai báo các tham số hình thức])   
 
        {    
            [Khai báo các biến cục bộ]    
            [Các câu lệnh]   
            [return[biểu thức];]   
            
         }   

 
Giải thích:   

-    `<Kiểu_trả_về>`: giá trị kiểu dữ liệu của dữ liệu sẽ trả về cho hàm   

-    `<tên_hàm>`: tên của hàm mà bạn muốn định nghĩa, được đặt theo qui tắc đặt tên của C   

-     [khai báo các tham số hình thức]: các tham số hình thức và kiểu của chúng    

-     [Khai báo các biến cục bộ]: khai báo các biến cục bộ, các biến này chỉ có tác dụng trong nội bộ hàm    

-     [return]: là lệnh thực hiện gán giá trị trả về cho hàm    

-      [biểu thức]: là giá trị trả về cho hàm, có thể là biến, hằng, biểu thức nhưng phải có giá trị xác định và có kiểu dữ liệu là kiểu đã khai báo cho hàm.   
```````````````````
ví dụ: Hàm tìm giá trị lớn nhất giữa hai giá trị
 
int tim_max(int a, int b);
{
            if(a>=b)
                        return a;
            else
                        return b;
}

``````````````````

*chú ý: 

- Hàm có thể có giá trị trả về hoặc không, giá trị trả về phải cùng kiểu với kiểu trả về đã khai báo hàm. Nếu hàm không có giá trị trả về thì đặt từ khóa void trước tên hàm để báo hiệu là hàm không cần giá trị trả về cho hàm.   

- Khi hàm khai báo không có kiểu ở trước nó thì nó được mặc định là kiểu int.   

- Không nhất thiết phải khai báo nguyên mẫu hàm. Nhưng nói chung nên có vì nó cho phép chương trình biên dịch phát hiện lỗi khi gọi.   

- Nguyên mẫu của hàm thực chất là dòng đầu tiên của hàm thêm vào dấu;. Tuy nhiên, trong nguyên mẫu có thể bỏ tên các tham số hình thức.   

####*II.HÀM VÀ CON TRỎ*  
-Đối số của hàm là con trỏ kiểu nào thì tham số thực tương ứng phải là địa chỉ của biến kiểu đó.Khi đó địa chỉ của biến được truyền cho đối con trỏ tương ứng.vd: Đối số của hàm là con trỏ kiểu int thì tham số thực tương ứng là địa chỉ của biến kiểu int    

 -Khi muốn bảo lưu lại kết quả tính toán được của các đối số trong hàm để sử dụng cho chương trình gọi hàm có đối số thì chúng ta phải khai báo đối số của hàm là tham chiếu (con trỏ hay dạng địa chỉ).
