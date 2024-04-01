insert into `rakamin-fintask.kimia_farma.analisis` (transaction_id, date, customer_name, discount_percentage)
select transaction_id, date, customer_name, discount_percentage
from `rakamin-fintask.kimia_farma.final_transaction`

INSERT INTO `rakamin-fintask.kimia_farma.analisis2`
SELECT ds.branch_id, ds.branch_name, rs.branch_name
FROM `rakamin-fintask.kimia_farma.analisis2` AS ds
RIGHT JOIN `rakamin-fintask.kimia_farma.kantor_cabang` AS rs
ON ds.source_join_branch_id = rs.right_join_branch_id

