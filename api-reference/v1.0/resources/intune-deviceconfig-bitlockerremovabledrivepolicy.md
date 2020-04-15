---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 78ce6f77c90e3b9356ccc75a6a202a9983b11874
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449101"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="64b59-103">bitLockerRemovableDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="64b59-103">bitLockerRemovableDrivePolicy resource type</span></span>

<span data-ttu-id="64b59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64b59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64b59-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="64b59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64b59-106">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="64b59-106">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="64b59-107">属性</span><span class="sxs-lookup"><span data-stu-id="64b59-107">Properties</span></span>
|<span data-ttu-id="64b59-108">属性</span><span class="sxs-lookup"><span data-stu-id="64b59-108">Property</span></span>|<span data-ttu-id="64b59-109">类型</span><span class="sxs-lookup"><span data-stu-id="64b59-109">Type</span></span>|<span data-ttu-id="64b59-110">说明</span><span class="sxs-lookup"><span data-stu-id="64b59-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64b59-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="64b59-111">encryptionMethod</span></span>|[<span data-ttu-id="64b59-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="64b59-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="64b59-113">选择可移动驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="64b59-113">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="64b59-114">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="64b59-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="64b59-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="64b59-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="64b59-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="64b59-116">Boolean</span></span>|<span data-ttu-id="64b59-117">指示是否阻止对其他组织中配置的设备的写入权限。</span><span class="sxs-lookup"><span data-stu-id="64b59-117">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="64b59-118">如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。</span><span class="sxs-lookup"><span data-stu-id="64b59-118">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="64b59-119">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="64b59-119">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="64b59-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="64b59-120">Boolean</span></span>|<span data-ttu-id="64b59-121">此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。</span><span class="sxs-lookup"><span data-stu-id="64b59-121">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64b59-122">关系</span><span class="sxs-lookup"><span data-stu-id="64b59-122">Relationships</span></span>
<span data-ttu-id="64b59-123">无</span><span class="sxs-lookup"><span data-stu-id="64b59-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64b59-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64b59-124">JSON Representation</span></span>
<span data-ttu-id="64b59-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64b59-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRemovableDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "blockCrossOrganizationWriteAccess": true
}
```







