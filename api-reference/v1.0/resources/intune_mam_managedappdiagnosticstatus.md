# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="2af42-101">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="2af42-101">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="2af42-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2af42-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2af42-103">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="2af42-103">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="2af42-104">属性</span><span class="sxs-lookup"><span data-stu-id="2af42-104">Properties</span></span>
|<span data-ttu-id="2af42-105">属性</span><span class="sxs-lookup"><span data-stu-id="2af42-105">Property</span></span>|<span data-ttu-id="2af42-106">类型</span><span class="sxs-lookup"><span data-stu-id="2af42-106">Type</span></span>|<span data-ttu-id="2af42-107">说明</span><span class="sxs-lookup"><span data-stu-id="2af42-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2af42-108">validationName</span><span class="sxs-lookup"><span data-stu-id="2af42-108">validationName</span></span>|<span data-ttu-id="2af42-109">String</span><span class="sxs-lookup"><span data-stu-id="2af42-109">String</span></span>|<span data-ttu-id="2af42-110">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="2af42-110">The validation friendly name</span></span>|
|<span data-ttu-id="2af42-111">状态</span><span class="sxs-lookup"><span data-stu-id="2af42-111">state</span></span>|<span data-ttu-id="2af42-112">String</span><span class="sxs-lookup"><span data-stu-id="2af42-112">String</span></span>|<span data-ttu-id="2af42-113">操作状态</span><span class="sxs-lookup"><span data-stu-id="2af42-113">The state of the operation</span></span>|
|<span data-ttu-id="2af42-114">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="2af42-114">mitigationInstruction</span></span>|<span data-ttu-id="2af42-115">String</span><span class="sxs-lookup"><span data-stu-id="2af42-115">String</span></span>|<span data-ttu-id="2af42-116">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="2af42-116">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="2af42-117">关系</span><span class="sxs-lookup"><span data-stu-id="2af42-117">Relationships</span></span>
<span data-ttu-id="2af42-118">无</span><span class="sxs-lookup"><span data-stu-id="2af42-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2af42-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2af42-119">JSON Representation</span></span>
<span data-ttu-id="2af42-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2af42-120">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```



