---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8017ac803ffa07a2e122553dee3268b0193157f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869571"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="0fa54-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="0fa54-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="0fa54-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0fa54-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0fa54-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0fa54-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0fa54-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0fa54-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0fa54-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0fa54-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0fa54-108">属性</span><span class="sxs-lookup"><span data-stu-id="0fa54-108">Properties</span></span>
|<span data-ttu-id="0fa54-109">属性</span><span class="sxs-lookup"><span data-stu-id="0fa54-109">Property</span></span>|<span data-ttu-id="0fa54-110">类型</span><span class="sxs-lookup"><span data-stu-id="0fa54-110">Type</span></span>|<span data-ttu-id="0fa54-111">说明</span><span class="sxs-lookup"><span data-stu-id="0fa54-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fa54-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="0fa54-112">deviceImportStatus</span></span>|[<span data-ttu-id="0fa54-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="0fa54-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="0fa54-114">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="0fa54-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="0fa54-115">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="0fa54-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="0fa54-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="0fa54-116">deviceRegistrationId</span></span>|<span data-ttu-id="0fa54-117">字符串</span><span class="sxs-lookup"><span data-stu-id="0fa54-117">String</span></span>|<span data-ttu-id="0fa54-118">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="0fa54-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="0fa54-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="0fa54-119">deviceErrorCode</span></span>|<span data-ttu-id="0fa54-120">Int32</span><span class="sxs-lookup"><span data-stu-id="0fa54-120">Int32</span></span>|<span data-ttu-id="0fa54-121">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="0fa54-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="0fa54-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="0fa54-122">deviceErrorName</span></span>|<span data-ttu-id="0fa54-123">字符串</span><span class="sxs-lookup"><span data-stu-id="0fa54-123">String</span></span>|<span data-ttu-id="0fa54-124">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="0fa54-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0fa54-125">关系</span><span class="sxs-lookup"><span data-stu-id="0fa54-125">Relationships</span></span>
<span data-ttu-id="0fa54-126">无</span><span class="sxs-lookup"><span data-stu-id="0fa54-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0fa54-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0fa54-127">JSON Representation</span></span>
<span data-ttu-id="0fa54-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0fa54-128">Here is a JSON representation of the resource.</span></span>
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





