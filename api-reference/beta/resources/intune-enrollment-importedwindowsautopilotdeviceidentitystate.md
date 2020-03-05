---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1af3f40e4e128272558b6fec75d5194ef48a9f6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528274"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="782a8-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="782a8-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="782a8-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="782a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="782a8-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="782a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="782a8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="782a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="782a8-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="782a8-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="782a8-108">属性</span><span class="sxs-lookup"><span data-stu-id="782a8-108">Properties</span></span>
|<span data-ttu-id="782a8-109">属性</span><span class="sxs-lookup"><span data-stu-id="782a8-109">Property</span></span>|<span data-ttu-id="782a8-110">类型</span><span class="sxs-lookup"><span data-stu-id="782a8-110">Type</span></span>|<span data-ttu-id="782a8-111">说明</span><span class="sxs-lookup"><span data-stu-id="782a8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="782a8-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="782a8-112">deviceImportStatus</span></span>|[<span data-ttu-id="782a8-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="782a8-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="782a8-114">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="782a8-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="782a8-115">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="782a8-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="782a8-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="782a8-116">deviceRegistrationId</span></span>|<span data-ttu-id="782a8-117">String</span><span class="sxs-lookup"><span data-stu-id="782a8-117">String</span></span>|<span data-ttu-id="782a8-118">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="782a8-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="782a8-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="782a8-119">deviceErrorCode</span></span>|<span data-ttu-id="782a8-120">Int32</span><span class="sxs-lookup"><span data-stu-id="782a8-120">Int32</span></span>|<span data-ttu-id="782a8-121">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="782a8-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="782a8-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="782a8-122">deviceErrorName</span></span>|<span data-ttu-id="782a8-123">字符串</span><span class="sxs-lookup"><span data-stu-id="782a8-123">String</span></span>|<span data-ttu-id="782a8-124">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="782a8-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="782a8-125">关系</span><span class="sxs-lookup"><span data-stu-id="782a8-125">Relationships</span></span>
<span data-ttu-id="782a8-126">无</span><span class="sxs-lookup"><span data-stu-id="782a8-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="782a8-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="782a8-127">JSON Representation</span></span>
<span data-ttu-id="782a8-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="782a8-128">Here is a JSON representation of the resource.</span></span>
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



