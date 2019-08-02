---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c5c474dc113d7d00bb0a43bef59c8196befddea3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028537"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="9ad9c-103">bitLockerRemovableDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ad9c-103">bitLockerRemovableDrivePolicy resource type</span></span>

> <span data-ttu-id="9ad9c-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ad9c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ad9c-105">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="9ad9c-105">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="9ad9c-106">属性</span><span class="sxs-lookup"><span data-stu-id="9ad9c-106">Properties</span></span>
|<span data-ttu-id="9ad9c-107">属性</span><span class="sxs-lookup"><span data-stu-id="9ad9c-107">Property</span></span>|<span data-ttu-id="9ad9c-108">类型</span><span class="sxs-lookup"><span data-stu-id="9ad9c-108">Type</span></span>|<span data-ttu-id="9ad9c-109">说明</span><span class="sxs-lookup"><span data-stu-id="9ad9c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ad9c-110">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="9ad9c-110">encryptionMethod</span></span>|[<span data-ttu-id="9ad9c-111">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="9ad9c-111">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="9ad9c-112">选择可移动驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="9ad9c-112">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="9ad9c-113">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="9ad9c-113">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="9ad9c-114">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="9ad9c-114">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="9ad9c-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ad9c-115">Boolean</span></span>|<span data-ttu-id="9ad9c-116">指示是否阻止对其他组织中配置的设备的写入权限。</span><span class="sxs-lookup"><span data-stu-id="9ad9c-116">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="9ad9c-117">如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。</span><span class="sxs-lookup"><span data-stu-id="9ad9c-117">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="9ad9c-118">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="9ad9c-118">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="9ad9c-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ad9c-119">Boolean</span></span>|<span data-ttu-id="9ad9c-120">此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。</span><span class="sxs-lookup"><span data-stu-id="9ad9c-120">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ad9c-121">关系</span><span class="sxs-lookup"><span data-stu-id="9ad9c-121">Relationships</span></span>
<span data-ttu-id="9ad9c-122">无</span><span class="sxs-lookup"><span data-stu-id="9ad9c-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ad9c-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ad9c-123">JSON Representation</span></span>
<span data-ttu-id="9ad9c-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ad9c-124">Here is a JSON representation of the resource.</span></span>
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



