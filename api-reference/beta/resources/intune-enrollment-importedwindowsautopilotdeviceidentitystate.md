---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
ms.openlocfilehash: cdb13df520d109ddcc49e2637652499186ac9f24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046310"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="e27e2-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="e27e2-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="e27e2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e27e2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e27e2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e27e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e27e2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e27e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e27e2-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e27e2-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="e27e2-108">属性</span><span class="sxs-lookup"><span data-stu-id="e27e2-108">Properties</span></span>
|<span data-ttu-id="e27e2-109">属性</span><span class="sxs-lookup"><span data-stu-id="e27e2-109">Property</span></span>|<span data-ttu-id="e27e2-110">类型</span><span class="sxs-lookup"><span data-stu-id="e27e2-110">Type</span></span>|<span data-ttu-id="e27e2-111">说明</span><span class="sxs-lookup"><span data-stu-id="e27e2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e27e2-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="e27e2-112">deviceImportStatus</span></span>|[<span data-ttu-id="e27e2-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="e27e2-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="e27e2-114">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="e27e2-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="e27e2-115">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="e27e2-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="e27e2-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="e27e2-116">deviceRegistrationId</span></span>|<span data-ttu-id="e27e2-117">字符串</span><span class="sxs-lookup"><span data-stu-id="e27e2-117">String</span></span>|<span data-ttu-id="e27e2-118">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="e27e2-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="e27e2-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="e27e2-119">deviceErrorCode</span></span>|<span data-ttu-id="e27e2-120">Int32</span><span class="sxs-lookup"><span data-stu-id="e27e2-120">Int32</span></span>|<span data-ttu-id="e27e2-121">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="e27e2-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="e27e2-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="e27e2-122">deviceErrorName</span></span>|<span data-ttu-id="e27e2-123">字符串</span><span class="sxs-lookup"><span data-stu-id="e27e2-123">String</span></span>|<span data-ttu-id="e27e2-124">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="e27e2-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e27e2-125">关系</span><span class="sxs-lookup"><span data-stu-id="e27e2-125">Relationships</span></span>
<span data-ttu-id="e27e2-126">无</span><span class="sxs-lookup"><span data-stu-id="e27e2-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e27e2-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e27e2-127">JSON Representation</span></span>
<span data-ttu-id="e27e2-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e27e2-128">Here is a JSON representation of the resource.</span></span>
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





