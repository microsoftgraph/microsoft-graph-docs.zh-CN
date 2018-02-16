# <a name="managedappdiagnosticstatus-resource-type"></a><span data-ttu-id="ca17e-101">managedAppDiagnosticStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca17e-101">managedAppDiagnosticStatus resource type</span></span>

> <span data-ttu-id="ca17e-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ca17e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca17e-103">表示诊断状态。</span><span class="sxs-lookup"><span data-stu-id="ca17e-103">Represents diagnostics status.</span></span>
## <a name="properties"></a><span data-ttu-id="ca17e-104">属性</span><span class="sxs-lookup"><span data-stu-id="ca17e-104">Properties</span></span>
|<span data-ttu-id="ca17e-105">属性</span><span class="sxs-lookup"><span data-stu-id="ca17e-105">Property</span></span>|<span data-ttu-id="ca17e-106">类型</span><span class="sxs-lookup"><span data-stu-id="ca17e-106">Type</span></span>|<span data-ttu-id="ca17e-107">说明</span><span class="sxs-lookup"><span data-stu-id="ca17e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca17e-108">validationName</span><span class="sxs-lookup"><span data-stu-id="ca17e-108">validationName</span></span>|<span data-ttu-id="ca17e-109">String</span><span class="sxs-lookup"><span data-stu-id="ca17e-109">String</span></span>|<span data-ttu-id="ca17e-110">验证友好名称</span><span class="sxs-lookup"><span data-stu-id="ca17e-110">The validation friendly name</span></span>|
|<span data-ttu-id="ca17e-111">状态</span><span class="sxs-lookup"><span data-stu-id="ca17e-111">state</span></span>|<span data-ttu-id="ca17e-112">String</span><span class="sxs-lookup"><span data-stu-id="ca17e-112">String</span></span>|<span data-ttu-id="ca17e-113">操作状态</span><span class="sxs-lookup"><span data-stu-id="ca17e-113">The state of a crawl operation.</span></span>|
|<span data-ttu-id="ca17e-114">mitigationInstruction</span><span class="sxs-lookup"><span data-stu-id="ca17e-114">mitigationInstruction</span></span>|<span data-ttu-id="ca17e-115">String</span><span class="sxs-lookup"><span data-stu-id="ca17e-115">String</span></span>|<span data-ttu-id="ca17e-116">有关如何降低失败验证的说明</span><span class="sxs-lookup"><span data-stu-id="ca17e-116">Instruction on how to mitigate a failed validation</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca17e-117">关系</span><span class="sxs-lookup"><span data-stu-id="ca17e-117">Relationships</span></span>
<span data-ttu-id="ca17e-118">无</span><span class="sxs-lookup"><span data-stu-id="ca17e-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ca17e-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca17e-119">JSON Representation</span></span>
<span data-ttu-id="ca17e-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca17e-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppDiagnosticStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppDiagnosticStatus",
  "validationName": "String",
  "state": "String",
  "mitigationInstruction": "String"
}
```



