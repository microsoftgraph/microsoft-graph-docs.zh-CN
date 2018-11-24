# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="63963-101">iosStoreAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="63963-101">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="63963-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="63963-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63963-103">包含用于为组分配 iOS 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="63963-103">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="63963-104">继承自 [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="63963-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="63963-105">属性</span><span class="sxs-lookup"><span data-stu-id="63963-105">Properties</span></span>
|<span data-ttu-id="63963-106">属性</span><span class="sxs-lookup"><span data-stu-id="63963-106">Property</span></span>|<span data-ttu-id="63963-107">类型</span><span class="sxs-lookup"><span data-stu-id="63963-107">Type</span></span>|<span data-ttu-id="63963-108">说明</span><span class="sxs-lookup"><span data-stu-id="63963-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63963-109">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="63963-109">vpnConfigurationId</span></span>|<span data-ttu-id="63963-110">String</span><span class="sxs-lookup"><span data-stu-id="63963-110">String</span></span>|<span data-ttu-id="63963-111">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="63963-111">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="63963-112">关系</span><span class="sxs-lookup"><span data-stu-id="63963-112">Relationships</span></span>
<span data-ttu-id="63963-113">无</span><span class="sxs-lookup"><span data-stu-id="63963-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="63963-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63963-114">JSON Representation</span></span>
<span data-ttu-id="63963-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63963-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



