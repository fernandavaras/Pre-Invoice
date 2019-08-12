
Select 

c.supplier_Cbn, h.*, m.*, PL.PL_CODE from wizadmin.company_profile c, wizadmin.wty_header h, wizadmin.monitoring_preinvoice m, WIZADMIN.PRODUCT_INFO pi, wizadmin.product_line pl    


where c.cust_id=m.cust_id  


and c.cust_id=h.cust_id  


and h.wty_id=m.wty_id  


and PL.PRODUCT_LINE_ID=PI.PRODUCT_LINE_ID  


and H.PRODUCT_NUMBER=PI.PRODUCT_NUMBER  


and M.PRODUCT_NUMBER=PI.PRODUCT_NUMBER  


and month='201907'  


and c.type in ('COMP_ASP','COMP_HP_SP')  


union  


Select 

c.supplier_Cbn, h.*, m.*, null from wizadmin.company_profile c, wizadmin.wty_header h, wizadmin.monitoring_preinvoice m 


where c.cust_id=m.cust_id  


and c.cust_id=h.cust_id  


and h.wty_id=m.wty_id  


and month='201907'  


and c.type in ('COMP_ASP','COMP_HP_SP') and h.wty_type ='WTYHTYPE_DOACLAIM' 
