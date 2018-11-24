# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="07779-101">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="07779-101">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="07779-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="07779-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07779-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="07779-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="07779-104">属性</span><span class="sxs-lookup"><span data-stu-id="07779-104">Properties</span></span>
|<span data-ttu-id="07779-105">属性</span><span class="sxs-lookup"><span data-stu-id="07779-105">Property</span></span>|<span data-ttu-id="07779-106">类型</span><span class="sxs-lookup"><span data-stu-id="07779-106">Type</span></span>|<span data-ttu-id="07779-107">说明</span><span class="sxs-lookup"><span data-stu-id="07779-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07779-108">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="07779-108">deviceImportStatus</span></span>|[<span data-ttu-id="07779-109">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="07779-109">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="07779-110">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="07779-110">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="07779-111">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="07779-111">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="07779-112">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="07779-112">deviceRegistrationId</span></span>|<span data-ttu-id="07779-113">字符串</span><span class="sxs-lookup"><span data-stu-id="07779-113">String</span></span>|<span data-ttu-id="07779-114">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="07779-114">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="07779-115">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="07779-115">deviceErrorCode</span></span>|<span data-ttu-id="07779-116">Int32</span><span class="sxs-lookup"><span data-stu-id="07779-116">Int32</span></span>|<span data-ttu-id="07779-117">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="07779-117">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="07779-118">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="07779-118">deviceErrorName</span></span>|<span data-ttu-id="07779-119">字符串</span><span class="sxs-lookup"><span data-stu-id="07779-119">String</span></span>|<span data-ttu-id="07779-120">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="07779-120">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="07779-121">关系</span><span class="sxs-lookup"><span data-stu-id="07779-121">Relationships</span></span>
<span data-ttu-id="07779-122">无</span><span class="sxs-lookup"><span data-stu-id="07779-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="07779-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07779-123">JSON Representation</span></span>
<span data-ttu-id="07779-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07779-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
  "deviceImportStatus": "String",
  "deviceRegistrationId": "String",
  "deviceErrorCode": 1024,
  "deviceErrorName": "String"
}
```



