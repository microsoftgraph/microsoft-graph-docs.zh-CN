---
title: bitlockerRecoveryKey 资源类型
description: BitLocker 恢复密钥资源
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 466a5d907b3deb589ec1b70351903e24aba0ab32
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443151"
---
# <a name="bitlockerrecoverykey-resource-type"></a><span data-ttu-id="e1ec5-103">bitlockerRecoveryKey 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1ec5-103">bitlockerRecoveryKey resource type</span></span>

<span data-ttu-id="e1ec5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1ec5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1ec5-105">表示通过键属性包含实际恢复密钥的已存储 BitLocker **密钥。**</span><span class="sxs-lookup"><span data-stu-id="e1ec5-105">Represents a stored BitLocker key that contains the actual recovery key via the **key** property.</span></span>

## <a name="methods"></a><span data-ttu-id="e1ec5-106">Methods</span><span class="sxs-lookup"><span data-stu-id="e1ec5-106">Methods</span></span>
|<span data-ttu-id="e1ec5-107">方法</span><span class="sxs-lookup"><span data-stu-id="e1ec5-107">Method</span></span>|<span data-ttu-id="e1ec5-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e1ec5-108">Return type</span></span>|<span data-ttu-id="e1ec5-109">说明</span><span class="sxs-lookup"><span data-stu-id="e1ec5-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e1ec5-110">列出 recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="e1ec5-110">List recoveryKeys</span></span>](../api/bitlocker-list-recoverykeys.md)|<span data-ttu-id="e1ec5-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1ec5-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span>|<span data-ttu-id="e1ec5-112">获取 [bitlockerRecoveryKey 对象及其](../resources/bitlockerrecoverykey.md) 属性的列表。</span><span class="sxs-lookup"><span data-stu-id="e1ec5-112">Get a list of the [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects and their properties.</span></span>|
|[<span data-ttu-id="e1ec5-113">获取 bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="e1ec5-113">Get bitlockerRecoveryKey</span></span>](../api/bitlockerrecoverykey-get.md)|[<span data-ttu-id="e1ec5-114">bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="e1ec5-114">bitlockerRecoveryKey</span></span>](../resources/bitlockerrecoverykey.md)|<span data-ttu-id="e1ec5-115">检索 [bitlockerRecoveryKey 对象的属性和](../resources/bitlockerrecoverykey.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="e1ec5-115">Retrieve the properties and relationships of a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object.</span></span> <span data-ttu-id="e1ec5-116">注意： **默认情况下** 不返回键属性。</span><span class="sxs-lookup"><span data-stu-id="e1ec5-116">Note: The **key** property is not returned by default.</span></span>|

> <span data-ttu-id="e1ec5-117">**注意**：只有某些角色具有调用这些 API 的权限。</span><span class="sxs-lookup"><span data-stu-id="e1ec5-117">**Note**: Only some roles have the permissions to call these APIs.</span></span>

## <a name="properties"></a><span data-ttu-id="e1ec5-118">属性</span><span class="sxs-lookup"><span data-stu-id="e1ec5-118">Properties</span></span>
|<span data-ttu-id="e1ec5-119">属性</span><span class="sxs-lookup"><span data-stu-id="e1ec5-119">Property</span></span>|<span data-ttu-id="e1ec5-120">类型</span><span class="sxs-lookup"><span data-stu-id="e1ec5-120">Type</span></span>|<span data-ttu-id="e1ec5-121">说明</span><span class="sxs-lookup"><span data-stu-id="e1ec5-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1ec5-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e1ec5-122">createdDateTime</span></span>|<span data-ttu-id="e1ec5-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1ec5-123">DateTimeOffset</span></span>|<span data-ttu-id="e1ec5-124">最初将密钥备份到 Azure Active Directory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e1ec5-124">The date and time when the key was originally backed up to Azure Active Directory.</span></span>|
|<span data-ttu-id="e1ec5-125">deviceId</span><span class="sxs-lookup"><span data-stu-id="e1ec5-125">deviceId</span></span>|<span data-ttu-id="e1ec5-126">String</span><span class="sxs-lookup"><span data-stu-id="e1ec5-126">String</span></span>|<span data-ttu-id="e1ec5-127">最初备份 BitLocker 密钥的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="e1ec5-127">ID of the device the BitLocker key is originally backed up from.</span></span>|
|<span data-ttu-id="e1ec5-128">id</span><span class="sxs-lookup"><span data-stu-id="e1ec5-128">id</span></span>|<span data-ttu-id="e1ec5-129">String</span><span class="sxs-lookup"><span data-stu-id="e1ec5-129">String</span></span>|<span data-ttu-id="e1ec5-130">BitLocker 密钥的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e1ec5-130">The unique identifier for the BitLocker key.</span></span>|
|<span data-ttu-id="e1ec5-131">注册表项</span><span class="sxs-lookup"><span data-stu-id="e1ec5-131">key</span></span>|<span data-ttu-id="e1ec5-132">String</span><span class="sxs-lookup"><span data-stu-id="e1ec5-132">String</span></span>|<span data-ttu-id="e1ec5-133">BitLocker 恢复密钥。</span><span class="sxs-lookup"><span data-stu-id="e1ec5-133">The BitLocker recovery key.</span></span>|
|<span data-ttu-id="e1ec5-134">volumeType</span><span class="sxs-lookup"><span data-stu-id="e1ec5-134">volumeType</span></span>|<span data-ttu-id="e1ec5-135">volumeType</span><span class="sxs-lookup"><span data-stu-id="e1ec5-135">volumeType</span></span>|<span data-ttu-id="e1ec5-136">指示 BitLocker 密钥关联的卷的类型。</span><span class="sxs-lookup"><span data-stu-id="e1ec5-136">Indicates the type of volume the BitLocker key is associated with.</span></span> <span data-ttu-id="e1ec5-137">可取值为：`operatingSystemVolume`、`fixedDataVolume`、`removableDataVolume`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="e1ec5-137">Possible values are: `operatingSystemVolume`, `fixedDataVolume`, `removableDataVolume`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1ec5-138">关系</span><span class="sxs-lookup"><span data-stu-id="e1ec5-138">Relationships</span></span>
<span data-ttu-id="e1ec5-139">无。</span><span class="sxs-lookup"><span data-stu-id="e1ec5-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1ec5-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1ec5-140">JSON representation</span></span>
<span data-ttu-id="e1ec5-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1ec5-141">The following is a JSON representation of the resource.</span></span>
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

