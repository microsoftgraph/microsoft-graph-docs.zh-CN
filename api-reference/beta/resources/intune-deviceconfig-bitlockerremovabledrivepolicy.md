---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b3a06b98ede0203a1bc76beb33a6565de439b99
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991042"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="4a8d6-103">bitLockerRemovableDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a8d6-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="4a8d6-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4a8d6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a8d6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a8d6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a8d6-106">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="4a8d6-106">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="4a8d6-107">属性</span><span class="sxs-lookup"><span data-stu-id="4a8d6-107">Properties</span></span>
|<span data-ttu-id="4a8d6-108">属性</span><span class="sxs-lookup"><span data-stu-id="4a8d6-108">Property</span></span>|<span data-ttu-id="4a8d6-109">类型</span><span class="sxs-lookup"><span data-stu-id="4a8d6-109">Type</span></span>|<span data-ttu-id="4a8d6-110">说明</span><span class="sxs-lookup"><span data-stu-id="4a8d6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a8d6-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="4a8d6-111">encryptionMethod</span></span>|[<span data-ttu-id="4a8d6-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="4a8d6-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="4a8d6-113">选择可移动驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="4a8d6-113">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="4a8d6-114">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="4a8d6-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="4a8d6-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="4a8d6-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="4a8d6-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a8d6-116">Boolean</span></span>|<span data-ttu-id="4a8d6-117">指示是否阻止对其他组织中配置的设备的写入权限。</span><span class="sxs-lookup"><span data-stu-id="4a8d6-117">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="4a8d6-118">如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。</span><span class="sxs-lookup"><span data-stu-id="4a8d6-118">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="4a8d6-119">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="4a8d6-119">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="4a8d6-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a8d6-120">Boolean</span></span>|<span data-ttu-id="4a8d6-121">此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。</span><span class="sxs-lookup"><span data-stu-id="4a8d6-121">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a8d6-122">关系</span><span class="sxs-lookup"><span data-stu-id="4a8d6-122">Relationships</span></span>
<span data-ttu-id="4a8d6-123">无</span><span class="sxs-lookup"><span data-stu-id="4a8d6-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a8d6-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a8d6-124">JSON Representation</span></span>
<span data-ttu-id="4a8d6-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a8d6-125">Here is a JSON representation of the resource.</span></span>
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





