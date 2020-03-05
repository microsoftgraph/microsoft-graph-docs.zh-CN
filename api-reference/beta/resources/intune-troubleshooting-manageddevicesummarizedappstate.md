---
title: managedDeviceSummarizedAppState 资源类型
description: 表示具有失败或挂起的应用程序的用户设备的事件。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: db00f874f6a2db1c4792955a3cbc2e5f32a81a0e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523357"
---
# <a name="manageddevicesummarizedappstate-resource-type"></a><span data-ttu-id="321b7-103">managedDeviceSummarizedAppState 资源类型</span><span class="sxs-lookup"><span data-stu-id="321b7-103">managedDeviceSummarizedAppState resource type</span></span>

<span data-ttu-id="321b7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="321b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="321b7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="321b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="321b7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="321b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="321b7-107">表示具有失败或挂起的应用程序的用户设备的事件。</span><span class="sxs-lookup"><span data-stu-id="321b7-107">Event representing a user's devices with failed or pending apps.</span></span>

## <a name="properties"></a><span data-ttu-id="321b7-108">属性</span><span class="sxs-lookup"><span data-stu-id="321b7-108">Properties</span></span>
|<span data-ttu-id="321b7-109">属性</span><span class="sxs-lookup"><span data-stu-id="321b7-109">Property</span></span>|<span data-ttu-id="321b7-110">类型</span><span class="sxs-lookup"><span data-stu-id="321b7-110">Type</span></span>|<span data-ttu-id="321b7-111">说明</span><span class="sxs-lookup"><span data-stu-id="321b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="321b7-112">summarizedAppState</span><span class="sxs-lookup"><span data-stu-id="321b7-112">summarizedAppState</span></span>|[<span data-ttu-id="321b7-113">runState</span><span class="sxs-lookup"><span data-stu-id="321b7-113">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="321b7-114">对象的 runState。</span><span class="sxs-lookup"><span data-stu-id="321b7-114">runState for the object.</span></span> <span data-ttu-id="321b7-115">可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。</span><span class="sxs-lookup"><span data-stu-id="321b7-115">Possible values are: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.</span></span>|
|<span data-ttu-id="321b7-116">deviceId</span><span class="sxs-lookup"><span data-stu-id="321b7-116">deviceId</span></span>|<span data-ttu-id="321b7-117">String</span><span class="sxs-lookup"><span data-stu-id="321b7-117">String</span></span>|<span data-ttu-id="321b7-118">此对象表示的设备的 DeviceId</span><span class="sxs-lookup"><span data-stu-id="321b7-118">DeviceId of device represented by this object</span></span>|

## <a name="relationships"></a><span data-ttu-id="321b7-119">关系</span><span class="sxs-lookup"><span data-stu-id="321b7-119">Relationships</span></span>
<span data-ttu-id="321b7-120">无</span><span class="sxs-lookup"><span data-stu-id="321b7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="321b7-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="321b7-121">JSON Representation</span></span>
<span data-ttu-id="321b7-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="321b7-122">Here is a JSON representation of the resource.</span></span>
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



