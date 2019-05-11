---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4f392f011f4bfcc615f88b6ea965fbc2b47899c9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941532"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="0a41f-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="0a41f-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="0a41f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0a41f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a41f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0a41f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a41f-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0a41f-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0a41f-107">属性</span><span class="sxs-lookup"><span data-stu-id="0a41f-107">Properties</span></span>
|<span data-ttu-id="0a41f-108">属性</span><span class="sxs-lookup"><span data-stu-id="0a41f-108">Property</span></span>|<span data-ttu-id="0a41f-109">类型</span><span class="sxs-lookup"><span data-stu-id="0a41f-109">Type</span></span>|<span data-ttu-id="0a41f-110">说明</span><span class="sxs-lookup"><span data-stu-id="0a41f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a41f-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="0a41f-111">deviceImportStatus</span></span>|[<span data-ttu-id="0a41f-112">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="0a41f-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="0a41f-113">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="0a41f-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="0a41f-114">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="0a41f-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="0a41f-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="0a41f-115">deviceRegistrationId</span></span>|<span data-ttu-id="0a41f-116">String</span><span class="sxs-lookup"><span data-stu-id="0a41f-116">String</span></span>|<span data-ttu-id="0a41f-117">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="0a41f-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="0a41f-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="0a41f-118">deviceErrorCode</span></span>|<span data-ttu-id="0a41f-119">Int32</span><span class="sxs-lookup"><span data-stu-id="0a41f-119">Int32</span></span>|<span data-ttu-id="0a41f-120">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="0a41f-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="0a41f-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="0a41f-121">deviceErrorName</span></span>|<span data-ttu-id="0a41f-122">字符串</span><span class="sxs-lookup"><span data-stu-id="0a41f-122">String</span></span>|<span data-ttu-id="0a41f-123">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="0a41f-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a41f-124">关系</span><span class="sxs-lookup"><span data-stu-id="0a41f-124">Relationships</span></span>
<span data-ttu-id="0a41f-125">无</span><span class="sxs-lookup"><span data-stu-id="0a41f-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a41f-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a41f-126">JSON Representation</span></span>
<span data-ttu-id="0a41f-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a41f-127">Here is a JSON representation of the resource.</span></span>
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




