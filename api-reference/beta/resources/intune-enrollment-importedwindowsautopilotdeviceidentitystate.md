---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b8130c354157bcfe679a95914e9266e500a6b51
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972941"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="0384f-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="0384f-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="0384f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0384f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0384f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0384f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0384f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0384f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0384f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0384f-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0384f-108">属性</span><span class="sxs-lookup"><span data-stu-id="0384f-108">Properties</span></span>
|<span data-ttu-id="0384f-109">属性</span><span class="sxs-lookup"><span data-stu-id="0384f-109">Property</span></span>|<span data-ttu-id="0384f-110">类型</span><span class="sxs-lookup"><span data-stu-id="0384f-110">Type</span></span>|<span data-ttu-id="0384f-111">说明</span><span class="sxs-lookup"><span data-stu-id="0384f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0384f-112">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="0384f-112">deviceImportStatus</span></span>|[<span data-ttu-id="0384f-113">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="0384f-113">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="0384f-114">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="0384f-114">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="0384f-115">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="0384f-115">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="0384f-116">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="0384f-116">deviceRegistrationId</span></span>|<span data-ttu-id="0384f-117">字符串</span><span class="sxs-lookup"><span data-stu-id="0384f-117">String</span></span>|<span data-ttu-id="0384f-118">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="0384f-118">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="0384f-119">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="0384f-119">deviceErrorCode</span></span>|<span data-ttu-id="0384f-120">Int32</span><span class="sxs-lookup"><span data-stu-id="0384f-120">Int32</span></span>|<span data-ttu-id="0384f-121">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="0384f-121">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="0384f-122">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="0384f-122">deviceErrorName</span></span>|<span data-ttu-id="0384f-123">字符串</span><span class="sxs-lookup"><span data-stu-id="0384f-123">String</span></span>|<span data-ttu-id="0384f-124">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="0384f-124">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="0384f-125">关系</span><span class="sxs-lookup"><span data-stu-id="0384f-125">Relationships</span></span>
<span data-ttu-id="0384f-126">无</span><span class="sxs-lookup"><span data-stu-id="0384f-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0384f-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0384f-127">JSON Representation</span></span>
<span data-ttu-id="0384f-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0384f-128">Here is a JSON representation of the resource.</span></span>
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





