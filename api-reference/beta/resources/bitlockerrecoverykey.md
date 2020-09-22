---
title: bitlockerRecoveryKey 资源类型
description: BitLocker 恢复密钥资源
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 038feb77f7ca57d426a44c04b3d9c93ae29e5aa4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081973"
---
# <a name="bitlockerrecoverykey-resource-type"></a><span data-ttu-id="d19f5-103">bitlockerRecoveryKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="d19f5-103">bitlockerRecoveryKey resource type</span></span>

<span data-ttu-id="d19f5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d19f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d19f5-105">表示一个存储的 BitLocker 密钥，其中包含通过 **key** 属性的实际恢复密钥。</span><span class="sxs-lookup"><span data-stu-id="d19f5-105">Represents a stored BitLocker key that contains the actual recovery key via the **key** property.</span></span>

## <a name="methods"></a><span data-ttu-id="d19f5-106">方法</span><span class="sxs-lookup"><span data-stu-id="d19f5-106">Methods</span></span>
|<span data-ttu-id="d19f5-107">方法</span><span class="sxs-lookup"><span data-stu-id="d19f5-107">Method</span></span>|<span data-ttu-id="d19f5-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d19f5-108">Return type</span></span>|<span data-ttu-id="d19f5-109">说明</span><span class="sxs-lookup"><span data-stu-id="d19f5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d19f5-110">列出 recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="d19f5-110">List recoveryKeys</span></span>](../api/bitlocker-list-recoverykeys.md)|<span data-ttu-id="d19f5-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d19f5-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span>|<span data-ttu-id="d19f5-112">获取 [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="d19f5-112">Get a list of the [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects and their properties.</span></span>|
|[<span data-ttu-id="d19f5-113">获取 bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="d19f5-113">Get bitlockerRecoveryKey</span></span>](../api/bitlockerrecoverykey-get.md)|[<span data-ttu-id="d19f5-114">bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="d19f5-114">bitlockerRecoveryKey</span></span>](../resources/bitlockerrecoverykey.md)|<span data-ttu-id="d19f5-115">检索 [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d19f5-115">Retrieve the properties and relationships of a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object.</span></span> <span data-ttu-id="d19f5-116">注意：默认情况下不返回 **key** 属性。</span><span class="sxs-lookup"><span data-stu-id="d19f5-116">Note: The **key** property is not returned by default.</span></span>|

> <span data-ttu-id="d19f5-117">**注意**：只有某些角色具有调用这些 api 的权限。</span><span class="sxs-lookup"><span data-stu-id="d19f5-117">**Note**: Only some roles have the permissions to call these APIs.</span></span>

## <a name="properties"></a><span data-ttu-id="d19f5-118">属性</span><span class="sxs-lookup"><span data-stu-id="d19f5-118">Properties</span></span>
|<span data-ttu-id="d19f5-119">属性</span><span class="sxs-lookup"><span data-stu-id="d19f5-119">Property</span></span>|<span data-ttu-id="d19f5-120">类型</span><span class="sxs-lookup"><span data-stu-id="d19f5-120">Type</span></span>|<span data-ttu-id="d19f5-121">说明</span><span class="sxs-lookup"><span data-stu-id="d19f5-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d19f5-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d19f5-122">createdDateTime</span></span>|<span data-ttu-id="d19f5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d19f5-123">DateTimeOffset</span></span>|<span data-ttu-id="d19f5-124">密钥最初备份到 Azure Active Directory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d19f5-124">The date and time when the key was originally backed up to Azure Active Directory.</span></span>|
|<span data-ttu-id="d19f5-125">deviceId</span><span class="sxs-lookup"><span data-stu-id="d19f5-125">deviceId</span></span>|<span data-ttu-id="d19f5-126">String</span><span class="sxs-lookup"><span data-stu-id="d19f5-126">String</span></span>|<span data-ttu-id="d19f5-127">BitLocker 密钥最初备份的设备的 ID。</span><span class="sxs-lookup"><span data-stu-id="d19f5-127">ID of the device the BitLocker key is originally backed up from.</span></span>|
|<span data-ttu-id="d19f5-128">id</span><span class="sxs-lookup"><span data-stu-id="d19f5-128">id</span></span>|<span data-ttu-id="d19f5-129">String</span><span class="sxs-lookup"><span data-stu-id="d19f5-129">String</span></span>|<span data-ttu-id="d19f5-130">BitLocker 密钥的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d19f5-130">The unique identifier for the BitLocker key.</span></span>|
|<span data-ttu-id="d19f5-131">注册表项</span><span class="sxs-lookup"><span data-stu-id="d19f5-131">key</span></span>|<span data-ttu-id="d19f5-132">String</span><span class="sxs-lookup"><span data-stu-id="d19f5-132">String</span></span>|<span data-ttu-id="d19f5-133">BitLocker 恢复密钥。</span><span class="sxs-lookup"><span data-stu-id="d19f5-133">The BitLocker recovery key.</span></span>|
|<span data-ttu-id="d19f5-134">volumeType</span><span class="sxs-lookup"><span data-stu-id="d19f5-134">volumeType</span></span>|<span data-ttu-id="d19f5-135">volumeType</span><span class="sxs-lookup"><span data-stu-id="d19f5-135">volumeType</span></span>|<span data-ttu-id="d19f5-136">指示与 BitLocker 密钥相关联的卷的类型。</span><span class="sxs-lookup"><span data-stu-id="d19f5-136">Indicates the type of volume the BitLocker key is associated with.</span></span> <span data-ttu-id="d19f5-137">可取值为：`operatingSystemVolume`、`fixedDataVolume`、`removableDataVolume`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d19f5-137">Possible values are: `operatingSystemVolume`, `fixedDataVolume`, `removableDataVolume`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d19f5-138">关系</span><span class="sxs-lookup"><span data-stu-id="d19f5-138">Relationships</span></span>
<span data-ttu-id="d19f5-139">无。</span><span class="sxs-lookup"><span data-stu-id="d19f5-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d19f5-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d19f5-140">JSON representation</span></span>
<span data-ttu-id="d19f5-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d19f5-141">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
  "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
  "createdDateTime": "2020-06-15T13:45:30.0000000Z",
  "volumeType": 1,
  "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9",
  "key": "123456-231453-873456-213546-654678-765689-123456-324565"
}
```

