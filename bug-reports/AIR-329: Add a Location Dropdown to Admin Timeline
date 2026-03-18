## ✅ QA Report – AIR-329: Location Filtering on Resource Timeline

### Environment
- Version: v0.25.2  
- Environment: Staging  
- URL: https://staging.airtopiapark.com/admin/booking/timeline  

### Browsers Tested
- Google Chrome  
- Safari (Desk + Mob) 
- Firefox  

---

### Test Summary
Location filtering on the Resource Timeline has been verified across multiple scenarios and browsers.  
Functionality works as expected with no data inconsistencies observed.

---

### Test Steps
1. Logged into Admin Panel  
2. Navigated to Resource Timeline  
3. Selected **Owasso** location → verified data  
4. Switched to **Tahlequah (T'quah)** → verified data updates  
5. Compared booking-related data between locations  

---

### Actual Result
- Timeline updates correctly based on selected location  
- No cross-location data leakage  
- Data corresponds to selected location  
- Behavior consistent across all tested browsers  

---

### Data Validation
- Verified booking number ranges differ per location  
- Confirms correct data isolation and filtering  

---

## ⚠️ QA Note (Risk & Recommendation)

Verified location filtering on Resource Timeline across Chrome, Safari, and Firefox.  
Data updates correctly per selected location with no cross-location leakage. No issues found.

Observed a potential risk: booking number ranges between locations are too close and may overlap over time. This could lead to confusion in reporting or data misinterpretation.

**Recommendation:** assign distinct number ranges per location:
- Owasso → 10000+  
- Tahlequah → 20000+  

This will:
- Ensure long-term scalability  
- Prevent overlap risks  
- Improve data clarity  

---

### Final Status
✅ **PASSED**
