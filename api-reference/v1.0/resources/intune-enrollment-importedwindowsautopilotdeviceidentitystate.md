---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 01524085500f8c8f8b313a9b2fbcbb89134de594
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030616"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="8d3c1-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="8d3c1-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="8d3c1-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d3c1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d3c1-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="8d3c1-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8d3c1-106">属性</span><span class="sxs-lookup"><span data-stu-id="8d3c1-106">Properties</span></span>
|<span data-ttu-id="8d3c1-107">属性</span><span class="sxs-lookup"><span data-stu-id="8d3c1-107">Property</span></span>|<span data-ttu-id="8d3c1-108">类型</span><span class="sxs-lookup"><span data-stu-id="8d3c1-108">Type</span></span>|<span data-ttu-id="8d3c1-109">说明</span><span class="sxs-lookup"><span data-stu-id="8d3c1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d3c1-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="8d3c1-110">deviceImportStatus</span></span>|[<span data-ttu-id="8d3c1-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="8d3c1-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="8d3c1-112">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="8d3c1-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="8d3c1-113">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="8d3c1-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="8d3c1-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="8d3c1-114">deviceRegistrationId</span></span>|<span data-ttu-id="8d3c1-115">String</span><span class="sxs-lookup"><span data-stu-id="8d3c1-115">String</span></span>|<span data-ttu-id="8d3c1-116">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="8d3c1-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="8d3c1-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="8d3c1-117">deviceErrorCode</span></span>|<span data-ttu-id="8d3c1-118">Int32</span><span class="sxs-lookup"><span data-stu-id="8d3c1-118">Int32</span></span>|<span data-ttu-id="8d3c1-119">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="8d3c1-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="8d3c1-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="8d3c1-120">deviceErrorName</span></span>|<span data-ttu-id="8d3c1-121">字符串</span><span class="sxs-lookup"><span data-stu-id="8d3c1-121">String</span></span>|<span data-ttu-id="8d3c1-122">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="8d3c1-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d3c1-123">关系</span><span class="sxs-lookup"><span data-stu-id="8d3c1-123">Relationships</span></span>
<span data-ttu-id="8d3c1-124">无</span><span class="sxs-lookup"><span data-stu-id="8d3c1-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d3c1-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8d3c1-125">JSON Representation</span></span>
<span data-ttu-id="8d3c1-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8d3c1-126">Here is a JSON representation of the resource.</span></span>
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



