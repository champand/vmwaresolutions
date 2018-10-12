---

copyright:

  years:  2016, 2018

lastupdated: "2018-09-21"

---

# 從 vCenter Server 實例中移除 Hybridity Bundle

若要從 vCenter Server 實例中移除 Hybridity Bundle 授權，您必須將 VMware NSX 及 VMware vSAN 租賃授權碼取代為 VMware vSphere Web Client 中的「自帶授權 (BYOL)」碼。此外，您還必須開立支援問題單，以取消租賃授權的費用。

**重要事項：**降級授權可能會導致 vCenter Server 實例失敗。您可以選擇自行承擔降級授權的風險，但是請先考量降級時無法使用的功能。如需相關資訊，請參閱 [VMware 元件版本的比較圖表](../archiref/solution/appendix.html)。

## 移除 Hybridity Bundle 之前

請先驗證下列需求，再移除 Hybridity Bundle：

* 您具有已啟用 Hybridity Bundle 的 2.4 版或更新版本的 vCenter Server 實例。
* 您的 vCenter Server 實例上未安裝 VMware HCX on {{site.data.keyword.cloud_notm}} 服務。
* 您以「管理者」身分存取 VMware vSphere Web Client。
* 如果尚未套用，則您有 BYOL 碼可用來申請 VMware NSX 及每個 VMware vSAN 叢集。
* （選擇性）如果尚未套用，則您有 BYOL 碼可用來申請 VMware vCenter Server 及 VMware vSphere Enterprise Plus 授權。

## 移除 Hybridity Bundle 的程序

1. 以**管理者**身分登入 VMware vSphere Web Client。
2. 按一下**首頁 > 管理 > 授權 > 授權**。
3. 按一下**資產**標籤。
4. 完成下列步驟，以安裝 VMware NSX BYOL：
   1. 按一下**解決方案**標籤。
   2. 選取 NSX for vSphere，然後按一下**所有動作 > 指派授權**。
   3. 按一下**新增**圖示，然後鍵入授權碼。按**下一步**。
   4. 鍵入授權的名稱，然後按**下一步**。按一下**完成**，以新增授權。
   5. 選取新的授權碼。
   6. 寫下所套用授權及所取代授權的完整授權碼。**重要事項：**您必須提供授權詳細資料，以供稍後在此程序中使用。
   7. 按一下**確定**，以指派授權。
5. 完成下列步驟，以安裝 VMware vSAN BYOL：
   1. 按一下**叢集**標籤。
   2. 針對與 vCenter Server 實例相關聯的每個 vSAN 叢集，完成下列步驟：
    1. 選取 vSAN 叢集，然後按一下**所有動作 > 指派授權**。
    2. 按一下**新增**圖示，然後鍵入授權碼。按**下一步**。
    3. 鍵入授權的名稱，然後按**下一步**。按一下**完成**，以新增授權。
    4. 選取新的授權碼。
    5. 寫下所套用授權及所取代授權的叢集名稱及完整授權碼。**重要事項：**您必須提供授權詳細資料，以供稍後在此程序中使用。
    6. 按一下**確定**，以指派授權。
6. 選擇性地完成下列步驟，以安裝 VMware vCenter Server BYOL：
   1. 按一下 **vCenter Server 系統**標籤。
   2. 選取 vCenter Server，然後按一下**所有動作 > 指派授權**。
   3. 按一下**新增**圖示，然後鍵入授權碼。按**下一步**。
   4. 鍵入授權的名稱，然後按**下一步**。按一下**完成**，以新增授權。
   5. 選取新的授權碼。
   6. 寫下所套用授權及所取代授權的完整授權碼。**重要事項：**您必須提供授權詳細資料，以供稍後在此程序中使用。
   7. 按一下**確定**，以指派授權。
7. 選擇性地完成下列步驟，以安裝 VMware vSphere Enterprise Plus BYOL：
  1. 按一下**主機**標籤。
  2. 針對與 vCenter Server 實例相關聯的每個叢集，完成下列步驟，或者，如果已將相同的授權套用至與 vCenter 伺服器相關聯的所有叢集，則同時針對所有叢集完成下列步驟：
    1. 選取所有與叢集相關聯的主機，然後按一下**所有動作 > 指派授權**。
    2. 按一下**新增**圖示，然後鍵入授權碼。按**下一步**。
    3. 鍵入授權的名稱，然後按**下一步**。按一下**完成**，以新增授權。
    4. 選取新的授權碼。
    5. 寫下所套用授權及所取代授權的叢集名稱及完整授權碼。**重要事項：**您必須提供授權詳細資料，以供稍後在此程序中使用。如果所有叢集的授權碼都不同，則請務必寫下與每個授權碼相關聯的叢集名稱。
    6. 按一下**確定**，以指派授權。
8. 移除租賃授權。
   1. 按一下**授權**標籤。
   2. 選取您在步驟 4 到 7 所取代的授權。
   3. 按一下**移除授權**圖示。
9. 開立支援問題單，並提供下列資訊來取消租賃授權的費用：
  * vCenter Server 實例的名稱。
  * 與 vCenter Server 實例相關聯的 ID。
  * 您在此程序中安裝的 BYOL 授權碼清單。如果適用，請提供具有 vSphere 及 vSAN 叢集授權碼的叢集名稱。
  * 您在此程序中移除的租賃授權碼清單。如果適用，請提供具有 vSphere 及 vSAN 叢集授權碼的叢集名稱。

  **附註：**「IBM 支援及作業」團隊可以存取 {{site.data.keyword.cloud_notm}} 基礎架構 (SoftLayer) 帳戶的 vCenter 管理層，以驗證已先移除租賃授權，再取消 Hybridity Bundle 租賃授權費用。

### 相關鏈結

* [訂購 vCenter Server with Hybridity Bundle 實例](vc_hybrid_orderinginstance.html)
* [檢視 vCenter Server with Hybridity Bundle 實例](vc_hybrid_viewinginstances.html)
* [與 IBM 支援中心聯絡](../vmonic/trbl_support.html)