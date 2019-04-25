---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e65de1501bb0480daf195ce910001624cabff98
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523362"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="0a0bc-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="0a0bc-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="0a0bc-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0a0bc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a0bc-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0a0bc-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0a0bc-106">属性</span><span class="sxs-lookup"><span data-stu-id="0a0bc-106">Properties</span></span>
|<span data-ttu-id="0a0bc-107">属性</span><span class="sxs-lookup"><span data-stu-id="0a0bc-107">Property</span></span>|<span data-ttu-id="0a0bc-108">类型</span><span class="sxs-lookup"><span data-stu-id="0a0bc-108">Type</span></span>|<span data-ttu-id="0a0bc-109">说明</span><span class="sxs-lookup"><span data-stu-id="0a0bc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a0bc-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="0a0bc-110">deviceImportStatus</span></span>|[<span data-ttu-id="0a0bc-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="0a0bc-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="0a0bc-112">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="0a0bc-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="0a0bc-113">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="0a0bc-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="0a0bc-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="0a0bc-114">deviceRegistrationId</span></span>|<span data-ttu-id="0a0bc-115">String</span><span class="sxs-lookup"><span data-stu-id="0a0bc-115">String</span></span>|<span data-ttu-id="0a0bc-116">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="0a0bc-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="0a0bc-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="0a0bc-117">deviceErrorCode</span></span>|<span data-ttu-id="0a0bc-118">Int32</span><span class="sxs-lookup"><span data-stu-id="0a0bc-118">Int32</span></span>|<span data-ttu-id="0a0bc-119">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="0a0bc-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="0a0bc-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="0a0bc-120">deviceErrorName</span></span>|<span data-ttu-id="0a0bc-121">字符串</span><span class="sxs-lookup"><span data-stu-id="0a0bc-121">String</span></span>|<span data-ttu-id="0a0bc-122">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="0a0bc-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a0bc-123">关系</span><span class="sxs-lookup"><span data-stu-id="0a0bc-123">Relationships</span></span>
<span data-ttu-id="0a0bc-124">无</span><span class="sxs-lookup"><span data-stu-id="0a0bc-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a0bc-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a0bc-125">JSON Representation</span></span>
<span data-ttu-id="0a0bc-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a0bc-126">Here is a JSON representation of the resource.</span></span>
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



