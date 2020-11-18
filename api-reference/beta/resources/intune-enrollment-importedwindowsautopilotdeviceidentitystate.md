---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8b9496c593cb714d830aa143918adcf87bed09c8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49197903"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="f2fab-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2fab-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

<span data-ttu-id="f2fab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2fab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2fab-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f2fab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2fab-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2fab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2fab-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f2fab-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f2fab-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2fab-108">Properties</span></span>
|<span data-ttu-id="f2fab-109">属性</span><span class="sxs-lookup"><span data-stu-id="f2fab-109">Property</span></span>|<span data-ttu-id="f2fab-110">类型</span><span class="sxs-lookup"><span data-stu-id="f2fab-110">Type</span></span>|<span data-ttu-id="f2fab-111">说明</span><span class="sxs-lookup"><span data-stu-id="f2fab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2fab-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="f2fab-112">deviceImportStatus</span></span>|[<span data-ttu-id="f2fab-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="f2fab-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="f2fab-114">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="f2fab-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="f2fab-115">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="f2fab-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="f2fab-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="f2fab-116">deviceRegistrationId</span></span>|<span data-ttu-id="f2fab-117">字符串</span><span class="sxs-lookup"><span data-stu-id="f2fab-117">String</span></span>|<span data-ttu-id="f2fab-118">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="f2fab-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="f2fab-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="f2fab-119">deviceErrorCode</span></span>|<span data-ttu-id="f2fab-120">Int32</span><span class="sxs-lookup"><span data-stu-id="f2fab-120">Int32</span></span>|<span data-ttu-id="f2fab-121">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="f2fab-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="f2fab-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="f2fab-122">deviceErrorName</span></span>|<span data-ttu-id="f2fab-123">字符串</span><span class="sxs-lookup"><span data-stu-id="f2fab-123">String</span></span>|<span data-ttu-id="f2fab-124">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="f2fab-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2fab-125">关系</span><span class="sxs-lookup"><span data-stu-id="f2fab-125">Relationships</span></span>
<span data-ttu-id="f2fab-126">无</span><span class="sxs-lookup"><span data-stu-id="f2fab-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2fab-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2fab-127">JSON Representation</span></span>
<span data-ttu-id="f2fab-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2fab-128">Here is a JSON representation of the resource.</span></span>
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




