# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="0b96a-101">microsoftStoreForBusinessAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b96a-101">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="0b96a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0b96a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b96a-103">包含用于为组分配适用于企业的 Microsoft 应用商店移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="0b96a-103">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="0b96a-104">继承自 [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="0b96a-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0b96a-105">属性</span><span class="sxs-lookup"><span data-stu-id="0b96a-105">Properties</span></span>
|<span data-ttu-id="0b96a-106">属性</span><span class="sxs-lookup"><span data-stu-id="0b96a-106">Property</span></span>|<span data-ttu-id="0b96a-107">类型</span><span class="sxs-lookup"><span data-stu-id="0b96a-107">Type</span></span>|<span data-ttu-id="0b96a-108">说明</span><span class="sxs-lookup"><span data-stu-id="0b96a-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b96a-109">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="0b96a-109">useDeviceContext</span></span>|<span data-ttu-id="0b96a-110">布尔值</span><span class="sxs-lookup"><span data-stu-id="0b96a-110">Boolean</span></span>|<span data-ttu-id="0b96a-111">是否要将设备执行上下文用于适用于企业的 Microsoft 应用商店移动应用。</span><span class="sxs-lookup"><span data-stu-id="0b96a-111">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b96a-112">关系</span><span class="sxs-lookup"><span data-stu-id="0b96a-112">Relationships</span></span>
<span data-ttu-id="0b96a-113">无</span><span class="sxs-lookup"><span data-stu-id="0b96a-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0b96a-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b96a-114">JSON Representation</span></span>
<span data-ttu-id="0b96a-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b96a-115">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.mobileAppAssignmentSettings",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```



