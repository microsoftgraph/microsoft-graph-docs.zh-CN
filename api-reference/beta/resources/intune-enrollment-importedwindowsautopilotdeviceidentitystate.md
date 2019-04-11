---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 42726817395296945fc593552ee50154fa34d332
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779767"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="2f13f-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f13f-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="2f13f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f13f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f13f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f13f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f13f-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2f13f-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2f13f-107">属性</span><span class="sxs-lookup"><span data-stu-id="2f13f-107">Properties</span></span>
|<span data-ttu-id="2f13f-108">属性</span><span class="sxs-lookup"><span data-stu-id="2f13f-108">Property</span></span>|<span data-ttu-id="2f13f-109">类型</span><span class="sxs-lookup"><span data-stu-id="2f13f-109">Type</span></span>|<span data-ttu-id="2f13f-110">说明</span><span class="sxs-lookup"><span data-stu-id="2f13f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f13f-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="2f13f-111">deviceImportStatus</span></span>|[<span data-ttu-id="2f13f-112">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="2f13f-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="2f13f-113">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="2f13f-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="2f13f-114">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="2f13f-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="2f13f-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="2f13f-115">deviceRegistrationId</span></span>|<span data-ttu-id="2f13f-116">String</span><span class="sxs-lookup"><span data-stu-id="2f13f-116">String</span></span>|<span data-ttu-id="2f13f-117">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="2f13f-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="2f13f-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="2f13f-118">deviceErrorCode</span></span>|<span data-ttu-id="2f13f-119">Int32</span><span class="sxs-lookup"><span data-stu-id="2f13f-119">Int32</span></span>|<span data-ttu-id="2f13f-120">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="2f13f-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="2f13f-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="2f13f-121">deviceErrorName</span></span>|<span data-ttu-id="2f13f-122">字符串</span><span class="sxs-lookup"><span data-stu-id="2f13f-122">String</span></span>|<span data-ttu-id="2f13f-123">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="2f13f-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f13f-124">关系</span><span class="sxs-lookup"><span data-stu-id="2f13f-124">Relationships</span></span>
<span data-ttu-id="2f13f-125">无</span><span class="sxs-lookup"><span data-stu-id="2f13f-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f13f-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f13f-126">JSON Representation</span></span>
<span data-ttu-id="2f13f-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f13f-127">Here is a JSON representation of the resource.</span></span>
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





