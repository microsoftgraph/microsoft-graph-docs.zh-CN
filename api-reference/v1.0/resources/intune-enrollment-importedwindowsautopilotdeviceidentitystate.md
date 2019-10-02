---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 841855ca7fb9de734fd685efa0d2382087256beb
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356833"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="8d8e7-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d8e7-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="8d8e7-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d8e7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d8e7-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8d8e7-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8d8e7-106">属性</span><span class="sxs-lookup"><span data-stu-id="8d8e7-106">Properties</span></span>
|<span data-ttu-id="8d8e7-107">属性</span><span class="sxs-lookup"><span data-stu-id="8d8e7-107">Property</span></span>|<span data-ttu-id="8d8e7-108">类型</span><span class="sxs-lookup"><span data-stu-id="8d8e7-108">Type</span></span>|<span data-ttu-id="8d8e7-109">说明</span><span class="sxs-lookup"><span data-stu-id="8d8e7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d8e7-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="8d8e7-110">deviceImportStatus</span></span>|[<span data-ttu-id="8d8e7-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="8d8e7-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="8d8e7-112">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="8d8e7-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="8d8e7-113">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="8d8e7-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="8d8e7-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="8d8e7-114">deviceRegistrationId</span></span>|<span data-ttu-id="8d8e7-115">String</span><span class="sxs-lookup"><span data-stu-id="8d8e7-115">String</span></span>|<span data-ttu-id="8d8e7-116">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="8d8e7-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="8d8e7-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="8d8e7-117">deviceErrorCode</span></span>|<span data-ttu-id="8d8e7-118">Int32</span><span class="sxs-lookup"><span data-stu-id="8d8e7-118">Int32</span></span>|<span data-ttu-id="8d8e7-119">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="8d8e7-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="8d8e7-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="8d8e7-120">deviceErrorName</span></span>|<span data-ttu-id="8d8e7-121">字符串</span><span class="sxs-lookup"><span data-stu-id="8d8e7-121">String</span></span>|<span data-ttu-id="8d8e7-122">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="8d8e7-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d8e7-123">关系</span><span class="sxs-lookup"><span data-stu-id="8d8e7-123">Relationships</span></span>
<span data-ttu-id="8d8e7-124">无</span><span class="sxs-lookup"><span data-stu-id="8d8e7-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d8e7-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d8e7-125">JSON Representation</span></span>
<span data-ttu-id="8d8e7-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d8e7-126">Here is a JSON representation of the resource.</span></span>
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




