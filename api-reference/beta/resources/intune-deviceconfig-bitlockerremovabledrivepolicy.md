---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 90d1bcb5464b6fbd1d31d0ddbc3f2bbd525d80d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527022"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="f9aff-103">bitLockerRemovableDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9aff-103">bitLockerRemovableDrivePolicy resource type</span></span>

<span data-ttu-id="f9aff-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f9aff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9aff-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f9aff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9aff-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9aff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9aff-107">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="f9aff-107">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="f9aff-108">属性</span><span class="sxs-lookup"><span data-stu-id="f9aff-108">Properties</span></span>
|<span data-ttu-id="f9aff-109">属性</span><span class="sxs-lookup"><span data-stu-id="f9aff-109">Property</span></span>|<span data-ttu-id="f9aff-110">类型</span><span class="sxs-lookup"><span data-stu-id="f9aff-110">Type</span></span>|<span data-ttu-id="f9aff-111">说明</span><span class="sxs-lookup"><span data-stu-id="f9aff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9aff-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="f9aff-112">encryptionMethod</span></span>|[<span data-ttu-id="f9aff-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="f9aff-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="f9aff-114">选择可移动驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="f9aff-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="f9aff-115">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="f9aff-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="f9aff-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="f9aff-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="f9aff-117">布尔</span><span class="sxs-lookup"><span data-stu-id="f9aff-117">Boolean</span></span>|<span data-ttu-id="f9aff-118">指示是否阻止对其他组织中配置的设备的写入权限。</span><span class="sxs-lookup"><span data-stu-id="f9aff-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="f9aff-119">如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。</span><span class="sxs-lookup"><span data-stu-id="f9aff-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="f9aff-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="f9aff-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="f9aff-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9aff-121">Boolean</span></span>|<span data-ttu-id="f9aff-122">此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。</span><span class="sxs-lookup"><span data-stu-id="f9aff-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9aff-123">关系</span><span class="sxs-lookup"><span data-stu-id="f9aff-123">Relationships</span></span>
<span data-ttu-id="f9aff-124">无</span><span class="sxs-lookup"><span data-stu-id="f9aff-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9aff-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9aff-125">JSON Representation</span></span>
<span data-ttu-id="f9aff-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9aff-126">Here is a JSON representation of the resource.</span></span>
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



