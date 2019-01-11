---
title: importedWindowsAutopilotDeviceIdentityState 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f6bb27b603669da82a42501563ad4be3220c7249
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870761"
---
# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a><span data-ttu-id="3a78b-103">importedWindowsAutopilotDeviceIdentityState 资源类型</span><span class="sxs-lookup"><span data-stu-id="3a78b-103">importedWindowsAutopilotDeviceIdentityState resource type</span></span>

> <span data-ttu-id="3a78b-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3a78b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3a78b-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="3a78b-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3a78b-106">属性</span><span class="sxs-lookup"><span data-stu-id="3a78b-106">Properties</span></span>
|<span data-ttu-id="3a78b-107">属性</span><span class="sxs-lookup"><span data-stu-id="3a78b-107">Property</span></span>|<span data-ttu-id="3a78b-108">类型</span><span class="sxs-lookup"><span data-stu-id="3a78b-108">Type</span></span>|<span data-ttu-id="3a78b-109">说明</span><span class="sxs-lookup"><span data-stu-id="3a78b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a78b-110">deviceImportStatus</span><span class="sxs-lookup"><span data-stu-id="3a78b-110">deviceImportStatus</span></span>|[<span data-ttu-id="3a78b-111">importedWindowsAutopilotDeviceIdentityImportStatus</span><span class="sxs-lookup"><span data-stu-id="3a78b-111">importedWindowsAutopilotDeviceIdentityImportStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)|<span data-ttu-id="3a78b-112">设备目录服务 (DDS) 报告的设备状态。</span><span class="sxs-lookup"><span data-stu-id="3a78b-112">Device status reported by Device Directory Service(DDS).</span></span> <span data-ttu-id="3a78b-113">可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="3a78b-113">Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.</span></span>|
|<span data-ttu-id="3a78b-114">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="3a78b-114">deviceRegistrationId</span></span>|<span data-ttu-id="3a78b-115">字符串</span><span class="sxs-lookup"><span data-stu-id="3a78b-115">String</span></span>|<span data-ttu-id="3a78b-116">设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。</span><span class="sxs-lookup"><span data-stu-id="3a78b-116">Device Registration ID for successfully added device reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="3a78b-117">deviceErrorCode</span><span class="sxs-lookup"><span data-stu-id="3a78b-117">deviceErrorCode</span></span>|<span data-ttu-id="3a78b-118">Int32</span><span class="sxs-lookup"><span data-stu-id="3a78b-118">Int32</span></span>|<span data-ttu-id="3a78b-119">设备目录服务 (DDS) 报告的设备错误代码。</span><span class="sxs-lookup"><span data-stu-id="3a78b-119">Device error code reported by Device Directory Service(DDS).</span></span>|
|<span data-ttu-id="3a78b-120">deviceErrorName</span><span class="sxs-lookup"><span data-stu-id="3a78b-120">deviceErrorName</span></span>|<span data-ttu-id="3a78b-121">字符串</span><span class="sxs-lookup"><span data-stu-id="3a78b-121">String</span></span>|<span data-ttu-id="3a78b-122">设备目录服务 (DDS) 报告的设备错误名称。</span><span class="sxs-lookup"><span data-stu-id="3a78b-122">Device error name reported by Device Directory Service(DDS).</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a78b-123">关系</span><span class="sxs-lookup"><span data-stu-id="3a78b-123">Relationships</span></span>
<span data-ttu-id="3a78b-124">无</span><span class="sxs-lookup"><span data-stu-id="3a78b-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3a78b-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a78b-125">JSON Representation</span></span>
<span data-ttu-id="3a78b-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a78b-126">Here is a JSON representation of the resource.</span></span>
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



