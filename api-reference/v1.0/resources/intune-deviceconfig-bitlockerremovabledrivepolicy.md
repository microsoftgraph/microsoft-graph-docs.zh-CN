---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d10a1039c0186238504836c0f719ab19ae4c4882
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261759"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="bf503-103">bitLockerRemovableDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf503-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="bf503-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf503-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf503-105">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="bf503-105">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="bf503-106">属性</span><span class="sxs-lookup"><span data-stu-id="bf503-106">Properties</span></span>
|<span data-ttu-id="bf503-107">属性</span><span class="sxs-lookup"><span data-stu-id="bf503-107">Property</span></span>|<span data-ttu-id="bf503-108">类型</span><span class="sxs-lookup"><span data-stu-id="bf503-108">Type</span></span>|<span data-ttu-id="bf503-109">说明</span><span class="sxs-lookup"><span data-stu-id="bf503-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf503-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="bf503-110">encryptionMethod</span></span>|[<span data-ttu-id="bf503-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="bf503-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="bf503-112">选择可移动驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="bf503-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="bf503-113">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="bf503-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="bf503-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="bf503-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="bf503-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf503-115">Boolean</span></span>|<span data-ttu-id="bf503-116">指示是否阻止对其他组织中配置的设备的写入权限。</span><span class="sxs-lookup"><span data-stu-id="bf503-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="bf503-117">如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。</span><span class="sxs-lookup"><span data-stu-id="bf503-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="bf503-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="bf503-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="bf503-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf503-119">Boolean</span></span>|<span data-ttu-id="bf503-120">此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。</span><span class="sxs-lookup"><span data-stu-id="bf503-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf503-121">关系</span><span class="sxs-lookup"><span data-stu-id="bf503-121">Relationships</span></span>
<span data-ttu-id="bf503-122">无</span><span class="sxs-lookup"><span data-stu-id="bf503-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf503-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf503-123">JSON Representation</span></span>
<span data-ttu-id="bf503-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf503-124">Here is a JSON representation of the resource.</span></span>
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



