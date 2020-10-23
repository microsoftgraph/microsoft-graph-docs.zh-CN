---
title: bitLockerRemovableDrivePolicy 资源类型
description: BitLocker 可移动驱动器策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 424fcdff8d2c16bbba1cba295bf626eeae7eda50
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697978"
---
# <a name="bitlockerremovabledrivepolicy-resource-type"></a><span data-ttu-id="3ba92-103">bitLockerRemovableDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ba92-103">bitLockerRemovableDrivePolicy resource type</span></span>

<span data-ttu-id="3ba92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ba92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3ba92-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3ba92-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ba92-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ba92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ba92-107">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="3ba92-107">BitLocker Removable Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="3ba92-108">属性</span><span class="sxs-lookup"><span data-stu-id="3ba92-108">Properties</span></span>
|<span data-ttu-id="3ba92-109">属性</span><span class="sxs-lookup"><span data-stu-id="3ba92-109">Property</span></span>|<span data-ttu-id="3ba92-110">类型</span><span class="sxs-lookup"><span data-stu-id="3ba92-110">Type</span></span>|<span data-ttu-id="3ba92-111">说明</span><span class="sxs-lookup"><span data-stu-id="3ba92-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ba92-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="3ba92-112">encryptionMethod</span></span>|[<span data-ttu-id="3ba92-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="3ba92-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="3ba92-114">选择可移动驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="3ba92-114">Select the encryption method for removable  drives.</span></span> <span data-ttu-id="3ba92-115">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="3ba92-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="3ba92-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="3ba92-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="3ba92-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ba92-117">Boolean</span></span>|<span data-ttu-id="3ba92-118">指示是否阻止对其他组织中配置的设备的写入权限。</span><span class="sxs-lookup"><span data-stu-id="3ba92-118">Indicates whether to block write access to devices configured in another organization.</span></span>  <span data-ttu-id="3ba92-119">如果 requireEncryptionForWriteAccess 为 false，则此值没有影响。</span><span class="sxs-lookup"><span data-stu-id="3ba92-119">If requireEncryptionForWriteAccess is false, this value does not affect.</span></span>|
|<span data-ttu-id="3ba92-120">blockCrossOrganizationWriteAccess</span><span class="sxs-lookup"><span data-stu-id="3ba92-120">blockCrossOrganizationWriteAccess</span></span>|<span data-ttu-id="3ba92-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="3ba92-121">Boolean</span></span>|<span data-ttu-id="3ba92-122">此策略设置决定可移动数据驱动器是否需要 BitLocker 保护，以使其在计算机上可写。</span><span class="sxs-lookup"><span data-stu-id="3ba92-122">This policy setting determines whether BitLocker protection is required for removable data drives to be writable on a computer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ba92-123">关系</span><span class="sxs-lookup"><span data-stu-id="3ba92-123">Relationships</span></span>
<span data-ttu-id="3ba92-124">无</span><span class="sxs-lookup"><span data-stu-id="3ba92-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ba92-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ba92-125">JSON Representation</span></span>
<span data-ttu-id="3ba92-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ba92-126">Here is a JSON representation of the resource.</span></span>
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





