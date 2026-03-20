## ✅ AIR-391 - Test Result

**Status:** Passed  
**Version:** v0.25.2  
**Environment:** Staging Guest Portal  

---

### Summary
Verified pricing behavior for Booking Bundle (e.g. *20 Flyer Private Table*) when adjusting guest count.

---

### Steps to Reproduce
1. Navigate to Guest Portal booking page  
2. Select a Booking Bundle  
3. Add it to cart  
4. Modify guest count within allowed range (e.g. 10–20)  

---

### Expected Result
Booking Bundle price remains **fixed** regardless of the number of guests.

---

### Actual Result
Booking Bundle price **does not change** when modifying the number of guests.

---

### Conclusion
The reported issue (bundle price being multiplied by guest count) is **not reproducible**.  
Pricing logic works as expected.
