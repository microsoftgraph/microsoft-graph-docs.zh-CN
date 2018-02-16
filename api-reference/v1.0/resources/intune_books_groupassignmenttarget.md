# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="7d505-101">groupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d505-101">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="7d505-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7d505-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d505-103">表示组的赋值。</span><span class="sxs-lookup"><span data-stu-id="7d505-103">Represents an assignment to a group.</span></span>

<span data-ttu-id="7d505-104">继承自 [deviceAndAppManagementAssignmentTarget](../resources/intune_books_deviceandappmanagementassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="7d505-104">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune_books_deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7d505-105">属性</span><span class="sxs-lookup"><span data-stu-id="7d505-105">Properties</span></span>
|<span data-ttu-id="7d505-106">属性</span><span class="sxs-lookup"><span data-stu-id="7d505-106">Property</span></span>|<span data-ttu-id="7d505-107">类型</span><span class="sxs-lookup"><span data-stu-id="7d505-107">Type</span></span>|<span data-ttu-id="7d505-108">说明</span><span class="sxs-lookup"><span data-stu-id="7d505-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d505-109">groupId</span><span class="sxs-lookup"><span data-stu-id="7d505-109">groupId</span></span>|<span data-ttu-id="7d505-110">String</span><span class="sxs-lookup"><span data-stu-id="7d505-110">String</span></span>|<span data-ttu-id="7d505-111">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="7d505-111">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d505-112">关系</span><span class="sxs-lookup"><span data-stu-id="7d505-112">Relationships</span></span>
<span data-ttu-id="7d505-113">无</span><span class="sxs-lookup"><span data-stu-id="7d505-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7d505-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d505-114">JSON Representation</span></span>
<span data-ttu-id="7d505-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d505-115">Here is a JSON representation of the resource.</span></span>
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



