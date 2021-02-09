---
title: usageRight 资源类型
description: 包含有关 usageRight 用户/设备已分配的信息
author: jeeshnair
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3f54fb6b54f08d28ab63bf2ec70180c5e0daf490
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159817"
---
# <a name="usageright-resource-type"></a><span data-ttu-id="0013b-103">usageRight 资源类型</span><span class="sxs-lookup"><span data-stu-id="0013b-103">usageRight resource type</span></span>

<span data-ttu-id="0013b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0013b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0013b-105">使用权限表示用户或设备具有的许可证，适用于基于电源应用构建的第三方软件，或仅针对基于设备 (订阅) 。</span><span class="sxs-lookup"><span data-stu-id="0013b-105">A usage right represents a license that a user or device has for either third party software built on power apps or for device based subscriptions (device only).</span></span>

## <a name="methods"></a><span data-ttu-id="0013b-106">方法</span><span class="sxs-lookup"><span data-stu-id="0013b-106">Methods</span></span>

|<span data-ttu-id="0013b-107">方法</span><span class="sxs-lookup"><span data-stu-id="0013b-107">Method</span></span>|<span data-ttu-id="0013b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="0013b-108">Return type</span></span>|<span data-ttu-id="0013b-109">说明</span><span class="sxs-lookup"><span data-stu-id="0013b-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0013b-110">列出用户 usageRights</span><span class="sxs-lookup"><span data-stu-id="0013b-110">List user usageRights</span></span>](../api/user-list-usagerights.md)|<span data-ttu-id="0013b-111">[usageRight](../resources/usageright.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0013b-111">[usageRight](../resources/usageright.md) collection</span></span>|<span data-ttu-id="0013b-112">获取用户的使用权限列表。</span><span class="sxs-lookup"><span data-stu-id="0013b-112">Get the list of usage rights for a user.</span></span>|
|[<span data-ttu-id="0013b-113">列出设备 usageRights</span><span class="sxs-lookup"><span data-stu-id="0013b-113">List device usageRights</span></span>](../api/device-list-usagerights.md)|<span data-ttu-id="0013b-114">[usageRight](../resources/usageright.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0013b-114">[usageRight](../resources/usageright.md) collection</span></span>|<span data-ttu-id="0013b-115">获取设备的使用权限列表。</span><span class="sxs-lookup"><span data-stu-id="0013b-115">Get the list of usage rights for a device.</span></span>|

## <a name="properties"></a><span data-ttu-id="0013b-116">属性</span><span class="sxs-lookup"><span data-stu-id="0013b-116">Properties</span></span>

|<span data-ttu-id="0013b-117">属性</span><span class="sxs-lookup"><span data-stu-id="0013b-117">Property</span></span>|<span data-ttu-id="0013b-118">类型</span><span class="sxs-lookup"><span data-stu-id="0013b-118">Type</span></span>|<span data-ttu-id="0013b-119">说明</span><span class="sxs-lookup"><span data-stu-id="0013b-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0013b-120">catalogId</span><span class="sxs-lookup"><span data-stu-id="0013b-120">catalogId</span></span>|<span data-ttu-id="0013b-121">String</span><span class="sxs-lookup"><span data-stu-id="0013b-121">String</span></span>|<span data-ttu-id="0013b-122">与使用权限对应的产品 ID。</span><span class="sxs-lookup"><span data-stu-id="0013b-122">Product id corresponding to the usage right.</span></span>|
|<span data-ttu-id="0013b-123">id</span><span class="sxs-lookup"><span data-stu-id="0013b-123">id</span></span>|<span data-ttu-id="0013b-124">String</span><span class="sxs-lookup"><span data-stu-id="0013b-124">String</span></span>|<span data-ttu-id="0013b-125">使用权限的 ID。</span><span class="sxs-lookup"><span data-stu-id="0013b-125">The id of the usage right.</span></span>|
|<span data-ttu-id="0013b-126">serviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="0013b-126">serviceIdentifier</span></span>|<span data-ttu-id="0013b-127">String</span><span class="sxs-lookup"><span data-stu-id="0013b-127">String</span></span>|<span data-ttu-id="0013b-128">与使用权限对应的服务的标识符。</span><span class="sxs-lookup"><span data-stu-id="0013b-128">Identifier of the service corresponding to the usage right.</span></span>|
|<span data-ttu-id="0013b-129">state</span><span class="sxs-lookup"><span data-stu-id="0013b-129">state</span></span>|<span data-ttu-id="0013b-130">usageRightState</span><span class="sxs-lookup"><span data-stu-id="0013b-130">usageRightState</span></span>|<span data-ttu-id="0013b-131">使用权限的状态。</span><span class="sxs-lookup"><span data-stu-id="0013b-131">The state of the usage right.</span></span> <span data-ttu-id="0013b-132">可取值为：`active`、`inactive`、`warning`、`suspended`。</span><span class="sxs-lookup"><span data-stu-id="0013b-132">Possible values are: `active`, `inactive`, `warning`, `suspended`.</span></span>|

### <a name="usagerightstate-values"></a><span data-ttu-id="0013b-133">usageRightState 值</span><span class="sxs-lookup"><span data-stu-id="0013b-133">usageRightState values</span></span> 

| <span data-ttu-id="0013b-134">成员</span><span class="sxs-lookup"><span data-stu-id="0013b-134">Member</span></span>             |  <span data-ttu-id="0013b-135">说明</span><span class="sxs-lookup"><span data-stu-id="0013b-135">Description</span></span>               |
| :----------------- |  :------------------------ |
|<span data-ttu-id="0013b-136">active</span><span class="sxs-lookup"><span data-stu-id="0013b-136">active</span></span>              | <span data-ttu-id="0013b-137">指示使用权限处于活动状态，可用于预配权益。</span><span class="sxs-lookup"><span data-stu-id="0013b-137">Indicates that the usage right is active and can be used for provisioning benefits.</span></span>|
|<span data-ttu-id="0013b-138">inactive</span><span class="sxs-lookup"><span data-stu-id="0013b-138">inactive</span></span>                | <span data-ttu-id="0013b-139">指示使用权限不是活动的，不能用于预配权益。</span><span class="sxs-lookup"><span data-stu-id="0013b-139">Indicates that the usage right is not active and cannot be used for provisioning benefits.</span></span>|
|<span data-ttu-id="0013b-140">警告</span><span class="sxs-lookup"><span data-stu-id="0013b-140">warning</span></span>                | <span data-ttu-id="0013b-141">指示使用权限可能由于付款违反而宽限期。</span><span class="sxs-lookup"><span data-stu-id="0013b-141">Indicates that the usage right is in grace likely due to payment violation.</span></span> <span data-ttu-id="0013b-142">此状态可用于提醒待付款或提供降级体验。</span><span class="sxs-lookup"><span data-stu-id="0013b-142">This state can be used to either remind of pending payment or offer a degraded experience.</span></span>|
|<span data-ttu-id="0013b-143">已挂起</span><span class="sxs-lookup"><span data-stu-id="0013b-143">suspended</span></span>                | <span data-ttu-id="0013b-144">指示使用权限可能由于付款违反而暂停</span><span class="sxs-lookup"><span data-stu-id="0013b-144">Indicates that the usage right is suspended likely due to Payment violation</span></span>|
|<span data-ttu-id="0013b-145">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="0013b-145">unknownFutureValue</span></span>      | <span data-ttu-id="0013b-146">指示未来值的 Sentinel 值。</span><span class="sxs-lookup"><span data-stu-id="0013b-146">Sentinel value to indicate future values.</span></span> |

><span data-ttu-id="0013b-147">**注意：** 只有活动状态和警告状态表示可用的好处。</span><span class="sxs-lookup"><span data-stu-id="0013b-147">**Note:** Only the active and warning states represent a usable benefit.</span></span> <span data-ttu-id="0013b-148">其他所有状态都将被视为没有产生可用的好处。</span><span class="sxs-lookup"><span data-stu-id="0013b-148">All other states should be treated as not resulting in a usable benefit.</span></span>



## <a name="relationships"></a><span data-ttu-id="0013b-149">关系</span><span class="sxs-lookup"><span data-stu-id="0013b-149">Relationships</span></span>

<span data-ttu-id="0013b-150">无。</span><span class="sxs-lookup"><span data-stu-id="0013b-150">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0013b-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0013b-151">JSON representation</span></span>

<span data-ttu-id="0013b-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0013b-152">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.usageRight",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.usageRight",
  "id": "String (identifier)",
  "catalogId": "String",
  "serviceIdentifier": "String",
  "state": "String"
}
```

