---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e65de1501bb0480daf195ce910001624cabff98
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261703"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="5ee7f-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ee7f-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="5ee7f-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ee7f-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="5ee7f-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5ee7f-106">属性</span><span class="sxs-lookup"><span data-stu-id="5ee7f-106">Properties</span></span>
|<span data-ttu-id="5ee7f-107">属性</span><span class="sxs-lookup"><span data-stu-id="5ee7f-107">Property</span></span>|<span data-ttu-id="5ee7f-108">类型</span><span class="sxs-lookup"><span data-stu-id="5ee7f-108">Type</span></span>|<span data-ttu-id="5ee7f-109">说明</span><span class="sxs-lookup"><span data-stu-id="5ee7f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ee7f-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="5ee7f-110">deviceImportStatus</span></span>|[<span data-ttu-id="5ee7f-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="5ee7f-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="5ee7f-112">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="5ee7f-113">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="5ee7f-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="5ee7f-114">deviceRegistrationId</span></span>|<span data-ttu-id="5ee7f-115">String</span><span class="sxs-lookup"><span data-stu-id="5ee7f-115">String</span></span>|<span data-ttu-id="5ee7f-116">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="5ee7f-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="5ee7f-117">deviceErrorCode</span></span>|<span data-ttu-id="5ee7f-118">Int32</span><span class="sxs-lookup"><span data-stu-id="5ee7f-118">Int32</span></span>|<span data-ttu-id="5ee7f-119">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="5ee7f-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="5ee7f-120">deviceErrorName</span></span>|<span data-ttu-id="5ee7f-121">字符串</span><span class="sxs-lookup"><span data-stu-id="5ee7f-121">String</span></span>|<span data-ttu-id="5ee7f-122">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ee7f-123">关系</span><span class="sxs-lookup"><span data-stu-id="5ee7f-123">Relationships</span></span>
<span data-ttu-id="5ee7f-124">无</span><span class="sxs-lookup"><span data-stu-id="5ee7f-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ee7f-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ee7f-125">JSON Representation</span></span>
<span data-ttu-id="5ee7f-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ee7f-126">Here is a JSON representation of the resource.</span></span>
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



