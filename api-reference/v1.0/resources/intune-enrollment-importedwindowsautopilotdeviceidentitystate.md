---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
ms.openlocfilehash: 6891c95a6c25c31c496c53520a22d5522995e29f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009914"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="979b6-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="979b6-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="979b6-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="979b6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="979b6-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="979b6-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="979b6-106">属性</span><span class="sxs-lookup"><span data-stu-id="979b6-106">Properties</span></span>
|<span data-ttu-id="979b6-107">属性</span><span class="sxs-lookup"><span data-stu-id="979b6-107">Property</span></span>|<span data-ttu-id="979b6-108">类型</span><span class="sxs-lookup"><span data-stu-id="979b6-108">Type</span></span>|<span data-ttu-id="979b6-109">说明</span><span class="sxs-lookup"><span data-stu-id="979b6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="979b6-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="979b6-110">deviceImportStatus</span></span>|[<span data-ttu-id="979b6-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="979b6-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="979b6-112">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="979b6-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="979b6-113">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="979b6-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="979b6-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="979b6-114">deviceRegistrationId</span></span>|<span data-ttu-id="979b6-115">字符串</span><span class="sxs-lookup"><span data-stu-id="979b6-115">String</span></span>|<span data-ttu-id="979b6-116">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="979b6-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="979b6-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="979b6-117">deviceErrorCode</span></span>|<span data-ttu-id="979b6-118">Int32</span><span class="sxs-lookup"><span data-stu-id="979b6-118">Int32</span></span>|<span data-ttu-id="979b6-119">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="979b6-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="979b6-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="979b6-120">deviceErrorName</span></span>|<span data-ttu-id="979b6-121">字符串</span><span class="sxs-lookup"><span data-stu-id="979b6-121">String</span></span>|<span data-ttu-id="979b6-122">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="979b6-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="979b6-123">关系</span><span class="sxs-lookup"><span data-stu-id="979b6-123">Relationships</span></span>
<span data-ttu-id="979b6-124">无</span><span class="sxs-lookup"><span data-stu-id="979b6-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="979b6-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="979b6-125">JSON Representation</span></span>
<span data-ttu-id="979b6-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="979b6-126">Here is a JSON representation of the resource.</span></span>
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



