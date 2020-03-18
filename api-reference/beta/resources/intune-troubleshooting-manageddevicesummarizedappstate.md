---
title: managedDeviceSummarizedAppState 资源类型
description: 表示具有失败或挂起的应用程序的用户设备的事件。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e6439ad781ad83bcae5bd66bc83f7a566e3b2ea6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42765151"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a><span data-ttu-id="96bff-103">managedDeviceSummarizedAppState 资源类型</span><span class="sxs-lookup"><span data-stu-id="96bff-103">managedDeviceSummarizedAppState resource type</span></span>

> <span data-ttu-id="96bff-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96bff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96bff-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96bff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96bff-106">表示具有失败或挂起的应用程序的用户设备的事件。</span><span class="sxs-lookup"><span data-stu-id="96bff-106">Event representing a user's devices with failed or pending apps.</span></span>

## <a name="properties"></a><span data-ttu-id="96bff-107">属性</span><span class="sxs-lookup"><span data-stu-id="96bff-107">Properties</span></span>
|<span data-ttu-id="96bff-108">属性</span><span class="sxs-lookup"><span data-stu-id="96bff-108">Property</span></span>|<span data-ttu-id="96bff-109">类型</span><span class="sxs-lookup"><span data-stu-id="96bff-109">Type</span></span>|<span data-ttu-id="96bff-110">说明</span><span class="sxs-lookup"><span data-stu-id="96bff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96bff-111">summarizedAppState</span><span class="sxs-lookup"><span data-stu-id="96bff-111">summarizedAppState</span></span>|[<span data-ttu-id="96bff-112">runState</span><span class="sxs-lookup"><span data-stu-id="96bff-112">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="96bff-113">对象的 runState。</span><span class="sxs-lookup"><span data-stu-id="96bff-113">runState for the object.</span></span> <span data-ttu-id="96bff-114">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="96bff-114">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="96bff-115">deviceId</span><span class="sxs-lookup"><span data-stu-id="96bff-115">deviceId</span></span>|<span data-ttu-id="96bff-116">String</span><span class="sxs-lookup"><span data-stu-id="96bff-116">String</span></span>|<span data-ttu-id="96bff-117">此对象表示的设备的 DeviceId</span><span class="sxs-lookup"><span data-stu-id="96bff-117">DeviceId of device represented by this object</span></span>|

## <a name="relationships"></a><span data-ttu-id="96bff-118">关系</span><span class="sxs-lookup"><span data-stu-id="96bff-118">Relationships</span></span>
<span data-ttu-id="96bff-119">无</span><span class="sxs-lookup"><span data-stu-id="96bff-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96bff-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96bff-120">JSON Representation</span></span>
<span data-ttu-id="96bff-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96bff-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceSummarizedAppState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceSummarizedAppState",
  "summarizedAppState": "String",
  "deviceId": "String"
}
```



