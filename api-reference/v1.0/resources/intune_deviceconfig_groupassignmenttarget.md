# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="b5a0f-101">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5a0f-101">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="b5a0f-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b5a0f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b5a0f-103">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="b5a0f-103">Represents an assignment to a group.</span></span>

<span data-ttu-id="b5a0f-104">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune_deviceconfig_deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="b5a0f-104">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune_deviceconfig_deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b5a0f-105">属性</span><span class="sxs-lookup"><span data-stu-id="b5a0f-105">Properties</span></span>
|<span data-ttu-id="b5a0f-106">属性</span><span class="sxs-lookup"><span data-stu-id="b5a0f-106">Property</span></span>|<span data-ttu-id="b5a0f-107">类型</span><span class="sxs-lookup"><span data-stu-id="b5a0f-107">Type</span></span>|<span data-ttu-id="b5a0f-108">说明</span><span class="sxs-lookup"><span data-stu-id="b5a0f-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5a0f-109">groupId</span><span class="sxs-lookup"><span data-stu-id="b5a0f-109">groupId</span></span>|<span data-ttu-id="b5a0f-110">String</span><span class="sxs-lookup"><span data-stu-id="b5a0f-110">String</span></span>|<span data-ttu-id="b5a0f-111">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="b5a0f-111">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5a0f-112">关系</span><span class="sxs-lookup"><span data-stu-id="b5a0f-112">Relationships</span></span>
<span data-ttu-id="b5a0f-113">无</span><span class="sxs-lookup"><span data-stu-id="b5a0f-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b5a0f-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5a0f-114">JSON Representation</span></span>
<span data-ttu-id="b5a0f-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5a0f-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```



