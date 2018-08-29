# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="3cbb0-101">exclusionGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="3cbb0-101">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="3cbb0-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3cbb0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3cbb0-103">表示应从赋值中排除的组。</span><span class="sxs-lookup"><span data-stu-id="3cbb0-103">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="3cbb0-104">继承自 [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="3cbb0-104">Inherits from [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3cbb0-105">属性</span><span class="sxs-lookup"><span data-stu-id="3cbb0-105">Properties</span></span>
|<span data-ttu-id="3cbb0-106">属性</span><span class="sxs-lookup"><span data-stu-id="3cbb0-106">Property</span></span>|<span data-ttu-id="3cbb0-107">类型</span><span class="sxs-lookup"><span data-stu-id="3cbb0-107">Type</span></span>|<span data-ttu-id="3cbb0-108">说明</span><span class="sxs-lookup"><span data-stu-id="3cbb0-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cbb0-109">groupId</span><span class="sxs-lookup"><span data-stu-id="3cbb0-109">groupId</span></span>|<span data-ttu-id="3cbb0-110">字符串</span><span class="sxs-lookup"><span data-stu-id="3cbb0-110">String</span></span>|<span data-ttu-id="3cbb0-111">赋值目标的组 ID。</span><span class="sxs-lookup"><span data-stu-id="3cbb0-111">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="3cbb0-112">继承自 [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="3cbb0-112">Inherited from [groupAssignmentTarget](../resources/intune_shared_groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cbb0-113">关系</span><span class="sxs-lookup"><span data-stu-id="3cbb0-113">Relationships</span></span>
<span data-ttu-id="3cbb0-114">无</span><span class="sxs-lookup"><span data-stu-id="3cbb0-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3cbb0-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3cbb0-115">JSON Representation</span></span>
<span data-ttu-id="3cbb0-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3cbb0-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.groupAssignmentTarget",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



