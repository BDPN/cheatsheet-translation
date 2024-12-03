**Linear Algebra and Calculus translation** [[webpage]](https://stanford.edu/~shervine/teaching/cs-229/refresher-algebra-calculus)

<br>

**1. Linear Algebra and Calculus refresher**

&#10230; 1. ทบทวนเนื้อหาพีชคณิตเชิงเส้นและแคลคูลัส

<br>

**2. General notations**

&#10230; 2. สัญกรณ์ทั่วไป

<br>

**3. Definitions**

&#10230; 3. นิยาม

<br>

**4. Vector ― We note x∈Rn a vector with n entries, where xi∈R is the ith entry:**

&#10230; 4. เวกเตอร์ (vector) ― ให้ x∈Rn เป็นเวกเตอร์ที่มีสมาชิก n ตัว โดย xi∈R แทนสมาชิกตัวที่ i

<br>

**5. Matrix ― We note A∈Rm×n a matrix with m rows and n columns, where Ai,j∈R is the entry located in the ith row and jth column:**

&#10230; 5. เมทริกซ์ (matrix) ― ให้ A∈Rm×n เป็นเมทริกซ์ที่มี m แถวและ n หลัก โดย Ai,j∈R คือสมาชิกที่อยู่ในแถวที่ i และหลักที่ j

<br>

**6. Remark: the vector x defined above can be viewed as a n×1 matrix and is more particularly called a column-vector.**

&#10230; 6. หมายเหตุ: เราสามารถมองเวกเตอร์ x ตามที่นิยามข้างต้นเป็นเมทริกซ์ขนาด n×1 และเรียกเป็นพิเศษว่าเวกเตอร์หลัก หรือเวกเตอร์แนวตั้ง (column vector)

> TL note
> 1. ปกติคำว่า "เวกเตอร์หลัก" กระชับกว่า แต่บางบริบทจะสับสนว่าคำว่า "หลัก" หมายถึง column หรือ main จึงมีอีกคำว่า "เวกเตอร์แนวตั้ง" ไว้ใช้สลับ
> 2. คำว่า remark หลายกรณีแปลว่า "ข้อสังเกต" แล้วเหมาะที่สุด แต่ในเอกสารนี้ ถัดลงไปเล็กน้อยที่ remark ที่ 3 จะเห็นกรณีที่คำว่า remark เป็น "สังเกต" ไม่ได้ เพราะเป็นข้อตกลงว่าจะใช้สัญลักษณ์อย่างหนึ่งๆ (ไม่ใช่สิ่งที่จะ "สังเกต" เอาเองได้) จึงคิดว่าหากจะแปล remark เป็นคำเดียวกันทั่วทั้งเอกสาร แปลว่า "หมายเหตุ" น่าจะเหมาะกว่า

<br>

**7. Main matrices**

&#10230; 7. เมทริกซ์หลักๆ

<br>

**8. Identity matrix ― The identity matrix I∈Rn×n is a square matrix with ones in its diagonal and zero everywhere else:**

&#10230; 8. เมทริกซ์เอกลักษณ์ (identity matrix) ― เมทริกซ์เอกลักษณ์ I∈Rn×n คือเมทริกซ์จัตุรัสที่แนวทแยงมุมเป็น 1 ส่วนตำแหน่งอื่นๆเป็น 0

<br>

**9. Remark: for all matrices A∈Rn×n, we have A×I=I×A=A.**

&#10230; 9. หมายเหตุ: ให้ A∈Rn×n เป็นเมทริกซ์ใดๆ จะได้ว่า A×I=I×A=A 

<br>

**10. Diagonal matrix ― A diagonal matrix D∈Rn×n is a square matrix with nonzero values in its diagonal and zero everywhere else:**

&#10230; 10. เมทริกซ์ทแยงมุม (diagonal matrix) ― เมทริกซ์ทแยงมุม D∈Rn×n คือเมทริกซ์จัตุรัสที่มีสมาชิกตามแนวทแยงมุมซึ่งไม่เป็น 0 ส่วนสมาชิกตัวอื่นๆที่เหลือเท่ากับ 0 

> TL note: ตีความว่านิยามในที่นี้หมายถึง "ต้องมีสมาชิกตามแนวทแยงมุมไม่เป็น 0 อย่างน้อยหนึ่งตัว" คาดว่านิยามเช่นนี้เพื่อตัดกรณี trivial ที่สมาชิกแนวทแยงมุมเป็น 0 ทั้งหมดออกไป เนื่องจากกรณีนั้นจะกลายเป็นเมทริกซ์ศูนย์แต่ต้น

<br>

**11. Remark: we also note D as diag(d1,...,dn).**

&#10230; 11. หมายเหตุ: เราเขียนแทน D ได้อีกแบบว่า diag(d1,...,dn)

<br>

**12. Matrix operations**

&#10230; 12. การกระทำของเมทริกซ์

<br>

**13. Multiplication**

&#10230; 13. การคูณ

<br>

**14. Vector-vector ― There are two types of vector-vector products:**

&#10230; 14. เวกเตอร์-เวกเตอร์ ― ผลคูณระหว่างเวกเตอร์กับเวกเตอร์มีสองแบบ

<br>

**15. inner product: for x,y∈Rn, we have:**

&#10230; 15. ผลคูณภายใน (inner product): ให้ x,y∈Rn จะได้ว่า:

<br>

**16. outer product: for x∈Rm,y∈Rn, we have:**

&#10230; 16. ผลคูณภายนอก (outer product): ให้ x∈Rm,y∈Rn จะได้ว่า:

<br>

**17. Matrix-vector ― The product of matrix A∈Rm×n and vector x∈Rn is a vector of size Rn, such that:**

&#10230; 17. เมทริกซ์-เวกเตอร์ ― ผลคูณของเมทริกซ์ A∈Rm×n กับเวกเตอร์ x∈Rn คือเวกเตอร์หนึ่งใน Rm ซึ่งมีสมบัติว่า:

> TL note: แปล "of size Rn" เป็น "ใน Rm" เพราะ Rm จริงๆเป็นเซตของเวกเตอร์ทั้งหมดที่มีขนาด m ถ้าจะใช้คำว่า "ขนาด" พูดว่า "เป็นเวกเตอร์ขนาด m" น่าจะเหมาะกว่า อนึ่ง สังเกตว่าแปลแก้จาก "[of size] Rn" เป็น "Rm" โดยยึดตามที่ปรากฏในหน้าเว็บ https://stanford.edu/~shervine/teaching/cs-229/refresher-algebra-calculus 

<br>

**18. where aTr,i are the vector rows and ac,j are the vector columns of A, and xi are the entries of x.**

&#10230; 18. เมื่อ aTr,i คือแต่ละแถวของ A เมื่อมองเป็นเวกเตอร์แนวนอน, ac,j คือแต่ละหลักของ A เมื่อมองเป็นเวกเตอร์แนวตั้ง, และ xi คือสมาชิกทั้งหลายของ x

> TL note: แปลแบบขยายความเพื่อให้เข้าใจง่ายขึ้น

<br>

**19. Matrix-matrix ― The product of matrices A∈Rm×n and B∈Rn×p is a matrix of size Rn×p, such that:**

&#10230; 19. เมทริกซ์-เมทริกซ์ ― ผลคูณของเมทริกซ์ A∈Rm×n กับ B∈Rn×p คือเมทริกซ์หนึ่งใน Rn×p ที่มีสมบัติว่า:

> TL note: แปล "of size Rn×p" เป็น "ใน Rn×p" เพราะ Rn×p จริงๆเป็นเซตของเมทริกซ์ทั้งหมดที่มีขนาด n×p ถ้าจะใช้คำว่า "ขนาด" พูดว่า "เป็นเวกเตอร์ขนาด n×p" น่าจะเหมาะกว่า

<br>

**20. where aTr,i,bTr,i are the vector rows and ac,j,bc,j are the vector columns of A and B respectively**

&#10230; 20. เมื่อ aTr,i,bTr,i คือแต่ละแถวของ A, B เมื่อมองเป็นเวกเตอร์, และ ac,j,bc,j คือแต่ละหลักของ A, B เมื่อมองเป็นเวกเตอร์

> TL note: แปลแบบขยายความเพื่อให้เข้าใจง่ายขึ้น

<br>

**21. Other operations**

&#10230; 21. การกระทำอื่นๆ

<br>

**22. Transpose ― The transpose of a matrix A∈Rm×n, noted AT, is such that its entries are flipped:**

&#10230; 22. ทรานส์โพส (transpose) ― เมทริกซ์ทรานซ์โพส (เมทริกซ์สลับเปลี่ยน) ของเมทริกซ์ A∈Rm×n ใช้สัญลักษณ์ว่า AT คือเมทริกซ์ A ที่สมาชิกอยู่ตำแหน่งพลิกสลับแถวกับหลักกัน

<br>

**23. Remark: for matrices A,B, we have (AB)T=BTAT**

&#10230; 23. ให้ A,B เป็นเมทริกซ์ จะได้ว่า (AB)T=BTAT

<br>

**24. Inverse ― The inverse of an invertible square matrix A is noted A−1 and is the only matrix such that:**

&#10230; อินเวอร์ส (inverse) ― อินเวอร์ส (ตัวผกผัน) ของเมทริกซ์จัตุรัส A หนึ่งๆซึ่งหาตัวผกผันได้ (invertible) ใช้สัญลักษณ์ว่า A−1 คือเมทริกซ์หนึ่งเดียวที่มีสมบัติว่า:

<br>

**25. Remark: not all square matrices are invertible. Also, for matrices A,B, we have (AB)−1=B−1A−1**

&#10230; 25. หมายเหตุ: เมทริกซ์จัตุรัสไม่ได้หาตัวผกผันได้ทุกเมทริกซ์เสมอไป และถ้า A,B เป็นเมทริกซ์ จะได้ว่า (AB)−1=B−1A−1

<br>

**26. Trace ― The trace of a square matrix A, noted tr(A), is the sum of its diagonal entries:**

&#10230; 26. เทรซ (trace) ― เทรซของเมทริกซ์จัตุรัส A หนึ่งๆ ใช้สัญลักษณ์ว่า tr(A) คือผลบวกของสมาชิกตามแนวทแยงมุมทุกตัว

> TL note: เพิ่มคำว่า "ทุกตัว" เพื่อให้ชัดเจนขึ้น

<br>

**27. Remark: for matrices A,B, we have tr(AT)=tr(A) and tr(AB)=tr(BA)**

&#10230; 27. หมายเหตุ: ให้ A,B เป็นเมทริกซ์ จะได้ว่า tr(AT)=tr(A) และ tr(AB)=tr(BA)

<br>

**28. Determinant ― The determinant of a square matrix A∈Rn×n, noted |A| or det(A) is expressed recursively in terms of A∖i,∖j, which is the matrix A without its ith row and jth column, as follows:**

&#10230; 28. ดีเทอร์มิแนนต์ (determinant) ― ดีเทอร์มิแนนต์ของเมทริกซ์จัตุรัส A∈Rn×n หนึ่งๆ ใช้สัญลักษณ์ว่า |A| หรือ det(A) นิยามในลักษณะเวียนเกิดดังนี้ อนึ่ง A∖i,∖j หมายถึงเมทริกซ์ A ที่ตัดแถวที่ i และหลักที่ j ออก:

<br>

**29. Remark: A is invertible if and only if |A|≠0. Also, |AB|=|A||B| and |AT|=|A|.**

&#10230; 29. หมายเหตุ: A หาตัวผกผันได้ก็ต่อเมื่อ |A|≠0 นอกจากนี้ |AB|=|A||B| และ |AT|=|A|

<br>

**30. Matrix properties**

&#10230; 30. สมบัติต่างๆของเมทริกซ์

<br>

**31. Definitions**

&#10230; 31. นิยาม

<br>

**32. Symmetric decomposition ― A given matrix A can be expressed in terms of its symmetric and antisymmetric parts as follows:**

&#10230; 32. การแยกเชิงสมมาตร (symmetric decomposition) ― เมทริกซ์ A หนึ่งๆสามารถเขียนในรูปส่วนที่สมมาตร (symmetric) กับปฏิสมมาตร (antisymmetric) ได้ดังนี้:

<br>

**33. [Symmetric, Antisymmetric]**

&#10230; 33. [สมมาตร, ปฏิสมมาตร]

<br>

**34. Norm ― A norm is a function N:V⟶[0,+∞[ where V is a vector space, and such that for all x,y∈V, we have:**

&#10230; 34. นอร์ม (norm) ― ให้ V เป็นปริภูมิเวกเตอร์ (vector space) นอร์มคือฟังก์ชัน N:V⟶[0,+∞[ ฟังก์ชันหนึ่ง ซึ่งมีสมบัติว่าสำหรับ x,y∈V ใดๆ จะได้ว่า: 

> TL note: ในต้นฉบับใช้สัญลักษณ์ช่วงว่า [0,+∞[ แต่ที่ไทยน่าจะนิยมเขียนว่า [0,+∞) มากกว่า

<br>

**35. N(ax)=|a|N(x) for a scalar**

&#10230; 35. N(ax)=|a|N(x) เมื่อ a เป็นค่าสเกลาร์ (scalar)

<br>

**36. if N(x)=0, then x=0**

&#10230; 36. ถ้า N(x)=0 แล้ว x=0

<br>

**37. For x∈V, the most commonly used norms are summed up in the table below:**

&#10230; 37. ให้ x∈V นอร์มที่ใช้งานบ่อยที่สุดสรุปได้ดังตารางด้านล่าง:

<br>

**38. [Norm, Notation, Definition, Use case]**

&#10230; 38. [นอร์ม, สัญกรณ์, นิยาม, การใช้งาน]

<br>

**39. Linearly dependence ― A set of vectors is said to be linearly dependent if one of the vectors in the set can be defined as a linear combination of the others.**

&#10230; 39. ความไม่เป็นอิสระเชิงเส้น (linearly dependence) ― เรากล่าวว่าเวกเตอร์ชุดหนึ่งไม่เป็นอิสระเชิงเส้น (linearly dependent) หากว่ามีเวกเตอร์หนึ่งในชุดนั้นสามารถเขียนในรูปผลรวมเชิงเส้นของเวกเตอร์อื่นๆในชุดได้

<br>

**40. Remark: if no vector can be written this way, then the vectors are said to be linearly independent**

&#10230; 40. หมายเหตุ: หากไม่มีเวกเตอร์ใดเลยเขียนได้ในลักษณะดังกล่าว เราจะกล่าวว่าเวกเตอร์เหล่านั้นเป็นอิสระเชิงเส้นต่อกัน

<br>

**41. Matrix rank ― The rank of a given matrix A is noted rank(A) and is the dimension of the vector space generated by its columns. This is equivalent to the maximum number of linearly independent columns of A.**

&#10230; 41. แรงก์ (rank) ของเมทริกซ์ ― ให้เมทริกซ์ A หนึ่งๆ หากมองแต่ละหลักของเมทริกซ์เป็นเวกเตอร์แนวตั้ง แล้วพิจารณาปริภูมิเวกเตอร์ที่ก่อกำเนิด (generated) จากเวกเตอร์แนวตั้งเหล่านั้นทั้งหมด แรงก์ของเมทริกซ์ A ใช้สัญลักษณ์ว่า rank(A) คือจำนวนมิติของปริภูมิเวกเตอร์ดังกล่าว ค่านี้เท่ากับจำนวนหลักของ A มากที่สุดที่เป็นอิสระเชิงเส้นต่อกัน

<br>

**42. Positive semi-definite matrix ― A matrix A∈Rn×n is positive semi-definite (PSD) and is noted A⪰0 if we have:**

&#10230; 42. เมทริกซ์เป็นบวกกึ่งแน่นอน (positive semi-definite matrix, PSD) ― เมทริกซ์ A∈Rn×n เป็นเมทริกซ์เป็นบวกกึ่งแน่นอน ใช้สัญลักษณ์ว่า A⪰0 หากว่าข้อความต่อไปนี้เป็นจริง:

> TL note: คำว่า "เป็นบวกกึ่งแน่นอน" อ้างอิงจากเอกสาร "พีชคณิตเชิงเส้น 1 (https://nithirungtanapirom.wordpress.com/wp-content/uploads/2023/11/2301234-linalg1-notes-2566-1.pdf)"

<br>

**43. Remark: similarly, a matrix A is said to be positive definite, and is noted A≻0, if it is a PSD matrix which satisfies for all non-zero vector x, xTAx>0.**

&#10230; 43. หมายเหตุ: ทำนองเดียวกัน เราจะกล่าวว่าเมทริกซ์ A เมทริกซ์หนึ่งเป็นบวกแน่นอน (positive definite) ใช้สัญลักษณ์ว่า A≻0 หากว่า A เป็นเมทริกซ์ PSD (เป็นบวกกึ่งแน่นอน) และ A สอดคล้องกับเงื่อนไขที่ว่าถ้า x เป็นเวกเตอร์ใดๆที่ไม่เป็นศูนย์แล้วเราได้ว่า xTAx>0

<br>

**44. Eigenvalue, eigenvector ― Given a matrix A∈Rn×n, λ is said to be an eigenvalue of A if there exists a vector z∈Rn∖{0}, called eigenvector, such that we have:**

&#10230; 44. ค่าเฉพาะ (eigenvalue), เวกเตอร์เฉพาะ (eigenvector) ― ให้เมทริกซ์ A∈Rn×n หนึ่งๆ เราจะกล่าวว่า λ เป็นค่าเฉพาะของ A หากว่ามีเวกเตอร์ z∈Rn∖{0} เรียกว่าเวกเตอร์เฉพาะ ซึ่งมีสมบัติว่า:

<br>

**45. Spectral theorem ― Let A∈Rn×n. If A is symmetric, then A is diagonalizable by a real orthogonal matrix U∈Rn×n. By noting Λ=diag(λ1,...,λn), we have:**

&#10230; 45. ทฤษฎีบทเชิงสเปคตรัม (spectral theorem) ― ให้ A∈Rn×n ถ้า A สมมาตร แล้ว A แปลงเป็นทแยงมุมได้ (diagonalizable) โดยใช้เมทริกซ์ U∈Rn×n หนึ่งซึ่งเป็นเมทริกซ์จริงเชิงตั้งฉาก (real orthogonal matrix) ในกรณีดังกล่าว หากให้ Λ=diag(λ1,...,λn) จะได้ว่า:

<br>

**46. diagonal**

&#10230; 46. (ตาม)แนวทแยงมุม

> TL note: ไม่แน่ใจว่า diagonal ในบริบทไหน คำนี้คำแปลที่เหมาะสุดอาจเปลี่ยนได้ตามบริบท

<br>

**47. Singular-value decomposition ― For a given matrix A of dimensions m×n, the singular-value decomposition (SVD) is a factorization technique that guarantees the existence of U m×m unitary, Σ m×n diagonal and V n×n unitary matrices, such that:**

&#10230; 47. การแยกค่าเอกฐาน (singular-value decomposition, SVD) ― ให้เมทริกซ์ A ขนาด m×n เมทริกซ์หนึ่ง การแยกค่าเอกฐานเป็นกลวิธีแยกตัวประกอบที่รับประกันว่าจะมีเมทริกซ์ยูนิแทรี (unitary) U ขนาด m×m, เมทริกซ์ทแยงมุม Σ ขนาด m×n, และเมทริกซ์ยูนิแทรี V ขนาด n×n ที่มีสมบัติว่า:

> TL note: คำว่า "แยกค่าเอกฐาน" พบที่เช่น http://cuir.car.chula.ac.th/handle/123456789/30091 และ https://phyblas.hinaboshi.com/20190916


<br>

**48. Matrix calculus**

&#10230; 48. แคลคูลัสเชิงเมทริกซ์

<br>

**49. Gradient ― Let f:Rm×n→R be a function and A∈Rm×n be a matrix. The gradient of f with respect to A is a m×n matrix, noted ∇Af(A), such that:**

&#10230; 49. เกรเดียนต์ (gradient) ― ให้ฟังก์ชัน f:Rm×n→R และเมทริกซ์ A∈Rm×n เกรเดียนต์ของ f เทียบกับ A คือเมทริกซ์ขนาด m×n เมทริกซ์หนึ่ง ใช้สัญลักษณ์ว่า ∇Af(A) ที่มีสมบัติว่า:

<br>

**50. Remark: the gradient of f is only defined when f is a function that returns a scalar.**

&#10230; 50. หมายเหตุ: เกรเดียนต์ของ f นิยามเฉพาะกรณีที่ f เป็นฟังก์ชันที่คืนค่าเป็นค่าสเกลาร์

<br>

**51. Hessian ― Let f:Rn→R be a function and x∈Rn be a vector. The hessian of f with respect to x is a n×n symmetric matrix, noted ∇2xf(x), such that:**

&#10230; 51. เฮสเซียน (Hessian) ― ให้ฟังก์ชัน f:Rn→R และเวกเตอร์ x∈Rn เฮสเซียนของ f เทียบกับ x คือเมทริกซ์สมมาตรขนาด n×n เมทริกซ์หนึ่ง ใช้สัญลักษณ์ว่า ∇2xf(x) ซึ่งมีสมบัติว่า:

<br> 

**52. Remark: the hessian of f is only defined when f is a function that returns a scalar**

&#10230; 52. หมายเหตุ: เฮสเซียนของ f นิยามเฉพาะกรณีที่ f เป็นฟังก์ชันที่คืนค่าเป็นค่าสเกลาร์

<br>

**53. Gradient operations ― For matrices A,B,C, the following gradient properties are worth having in mind:**

&#10230; 53. การกระทำของเกรเดียนต์ ― ให้ A,B,C เป็นเมทริกซ์ เกรเดียนต์มีสมบัติพึงจำดังนี้:

<br>

**54. [General notations, Definitions, Main matrices]**

&#10230; 54. [สัญกรณ์ทั่วไป, นิยาม, เมทริกซ์หลักๆ]

<br>

**55. [Matrix operations, Multiplication, Other operations]**

&#10230; 55. [การกระทำของเมทริกซ์, การคูณ, การกระทำอื่นๆ]

<br>

**56. [Matrix properties, Norm, Eigenvalue/Eigenvector, Singular-value decomposition]**

&#10230; 56. [สมบัติต่างๆของเมทริกซ์, นอร์ม, ค่าเฉพาะ/เวกเตอร์เฉพาะ, การแยกค่าเอกฐาน]

<br>

**57. [Matrix calculus, Gradient, Hessian, Operations]**

&#10230; 57. [แคลคูลัสเชิงเมทริกซ์, เกรเดียนต์, เฮสเซียน, การกระทำต่างๆ]
