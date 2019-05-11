---
title: bitLockerFixedDrivePolicy 资源类型
description: BitLocker 固定驱动器策略。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 326d9c873fd1e0b6b00656aa6b831b7e05ac6bf0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947517"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="4318f-103">bitLockerFixedDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="4318f-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="4318f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4318f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4318f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4318f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4318f-106">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="4318f-106">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="4318f-107">属性</span><span class="sxs-lookup"><span data-stu-id="4318f-107">Properties</span></span>
|<span data-ttu-id="4318f-108">属性</span><span class="sxs-lookup"><span data-stu-id="4318f-108">Property</span></span>|<span data-ttu-id="4318f-109">类型</span><span class="sxs-lookup"><span data-stu-id="4318f-109">Type</span></span>|<span data-ttu-id="4318f-110">说明</span><span class="sxs-lookup"><span data-stu-id="4318f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4318f-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="4318f-111">encryptionMethod</span></span>|[<span data-ttu-id="4318f-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="4318f-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="4318f-113">选择固定驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="4318f-113">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="4318f-114">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="4318f-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="4318f-115">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="4318f-115">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="4318f-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="4318f-116">Boolean</span></span>|<span data-ttu-id="4318f-117">此策略设置确定固定数据驱动器在计算机上是否可写, 是否需要 BitLocker 保护。</span><span class="sxs-lookup"><span data-stu-id="4318f-117">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="4318f-118">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="4318f-118">recoveryOptions</span></span>|[<span data-ttu-id="4318f-119">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="4318f-119">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="4318f-120">通过此策略设置, 您可以控制在缺少所需凭据的情况中恢复受 BitLocker 保护的固定数据驱动器的方式。</span><span class="sxs-lookup"><span data-stu-id="4318f-120">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="4318f-121">启用 BitLocker 时, 将应用此策略设置。</span><span class="sxs-lookup"><span data-stu-id="4318f-121">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4318f-122">关系</span><span class="sxs-lookup"><span data-stu-id="4318f-122">Relationships</span></span>
<span data-ttu-id="4318f-123">无</span><span class="sxs-lookup"><span data-stu-id="4318f-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4318f-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4318f-124">JSON Representation</span></span>
<span data-ttu-id="4318f-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4318f-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerFixedDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerFixedDrivePolicy",
  "encryptionMethod": "String",
  "requireEncryptionForWriteAccess": true,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  }
}
```




