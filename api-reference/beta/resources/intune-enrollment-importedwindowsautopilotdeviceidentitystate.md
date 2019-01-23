---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0f4e76b23d4d970a9fb873326dc84f278aa2ed2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410964"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="72b50-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="72b50-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="72b50-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="72b50-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="72b50-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="72b50-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="72b50-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72b50-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72b50-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="72b50-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="72b50-108">属性</span><span class="sxs-lookup"><span data-stu-id="72b50-108">Properties</span></span>
|<span data-ttu-id="72b50-109">属性</span><span class="sxs-lookup"><span data-stu-id="72b50-109">Property</span></span>|<span data-ttu-id="72b50-110">类型</span><span class="sxs-lookup"><span data-stu-id="72b50-110">Type</span></span>|<span data-ttu-id="72b50-111">说明</span><span class="sxs-lookup"><span data-stu-id="72b50-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72b50-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="72b50-112">deviceImportStatus</span></span>|[<span data-ttu-id="72b50-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="72b50-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="72b50-114">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="72b50-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="72b50-115">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="72b50-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="72b50-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="72b50-116">deviceRegistrationId</span></span>|<span data-ttu-id="72b50-117">字符串</span><span class="sxs-lookup"><span data-stu-id="72b50-117">String</span></span>|<span data-ttu-id="72b50-118">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="72b50-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="72b50-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="72b50-119">deviceErrorCode</span></span>|<span data-ttu-id="72b50-120">Int32</span><span class="sxs-lookup"><span data-stu-id="72b50-120">Int32</span></span>|<span data-ttu-id="72b50-121">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="72b50-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="72b50-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="72b50-122">deviceErrorName</span></span>|<span data-ttu-id="72b50-123">字符串</span><span class="sxs-lookup"><span data-stu-id="72b50-123">String</span></span>|<span data-ttu-id="72b50-124">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="72b50-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="72b50-125">关系</span><span class="sxs-lookup"><span data-stu-id="72b50-125">Relationships</span></span>
<span data-ttu-id="72b50-126">无</span><span class="sxs-lookup"><span data-stu-id="72b50-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72b50-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72b50-127">JSON Representation</span></span>
<span data-ttu-id="72b50-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72b50-128">Here is a JSON representation of the resource.</span></span>
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




