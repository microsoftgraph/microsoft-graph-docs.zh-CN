---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fe8ae3addc2d4b74323471bc39fd8d5569d4df99
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530244"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="f101a-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="f101a-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="f101a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f101a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f101a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f101a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f101a-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f101a-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f101a-107">属性</span><span class="sxs-lookup"><span data-stu-id="f101a-107">Properties</span></span>
|<span data-ttu-id="f101a-108">属性</span><span class="sxs-lookup"><span data-stu-id="f101a-108">Property</span></span>|<span data-ttu-id="f101a-109">类型</span><span class="sxs-lookup"><span data-stu-id="f101a-109">Type</span></span>|<span data-ttu-id="f101a-110">说明</span><span class="sxs-lookup"><span data-stu-id="f101a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f101a-111">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="f101a-111">deviceImportStatus</span></span>|[<span data-ttu-id="f101a-112">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="f101a-112">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="f101a-113">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="f101a-113">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="f101a-114">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="f101a-114">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="f101a-115">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="f101a-115">deviceRegistrationId</span></span>|<span data-ttu-id="f101a-116">字符串</span><span class="sxs-lookup"><span data-stu-id="f101a-116">String</span></span>|<span data-ttu-id="f101a-117">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="f101a-117">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="f101a-118">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="f101a-118">deviceErrorCode</span></span>|<span data-ttu-id="f101a-119">Int32</span><span class="sxs-lookup"><span data-stu-id="f101a-119">Int32</span></span>|<span data-ttu-id="f101a-120">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="f101a-120">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="f101a-121">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="f101a-121">deviceErrorName</span></span>|<span data-ttu-id="f101a-122">字符串</span><span class="sxs-lookup"><span data-stu-id="f101a-122">String</span></span>|<span data-ttu-id="f101a-123">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="f101a-123">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f101a-124">关系</span><span class="sxs-lookup"><span data-stu-id="f101a-124">Relationships</span></span>
<span data-ttu-id="f101a-125">无</span><span class="sxs-lookup"><span data-stu-id="f101a-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f101a-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f101a-126">JSON Representation</span></span>
<span data-ttu-id="f101a-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f101a-127">Here is a JSON representation of the resource.</span></span>
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




