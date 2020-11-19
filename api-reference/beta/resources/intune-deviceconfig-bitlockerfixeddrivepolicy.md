---
title: bitLockerFixedDrivePolicy 资源类型
description: BitLocker 固定驱动器策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 323d45fb8109820a74f6b0394431a297ed2618e6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260612"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="142d2-103">bitLockerFixedDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="142d2-103">bitLockerFixedDrivePolicy resource type</span></span>

<span data-ttu-id="142d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="142d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="142d2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="142d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="142d2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="142d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="142d2-107">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="142d2-107">BitLocker Fixed Drive Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="142d2-108">属性</span><span class="sxs-lookup"><span data-stu-id="142d2-108">Properties</span></span>
|<span data-ttu-id="142d2-109">属性</span><span class="sxs-lookup"><span data-stu-id="142d2-109">Property</span></span>|<span data-ttu-id="142d2-110">类型</span><span class="sxs-lookup"><span data-stu-id="142d2-110">Type</span></span>|<span data-ttu-id="142d2-111">描述</span><span class="sxs-lookup"><span data-stu-id="142d2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="142d2-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="142d2-112">encryptionMethod</span></span>|[<span data-ttu-id="142d2-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="142d2-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="142d2-114">选择固定驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="142d2-114">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="142d2-115">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="142d2-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="142d2-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="142d2-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="142d2-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="142d2-117">Boolean</span></span>|<span data-ttu-id="142d2-118">此策略设置确定固定数据驱动器在计算机上是否可写，是否需要 BitLocker 保护。</span><span class="sxs-lookup"><span data-stu-id="142d2-118">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="142d2-119">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="142d2-119">recoveryOptions</span></span>|[<span data-ttu-id="142d2-120">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="142d2-120">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="142d2-121">通过此策略设置，您可以控制在缺少所需凭据的情况中恢复受 BitLocker 保护的固定数据驱动器的方式。</span><span class="sxs-lookup"><span data-stu-id="142d2-121">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="142d2-122">启用 BitLocker 时，将应用此策略设置。</span><span class="sxs-lookup"><span data-stu-id="142d2-122">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="142d2-123">关系</span><span class="sxs-lookup"><span data-stu-id="142d2-123">Relationships</span></span>
<span data-ttu-id="142d2-124">无</span><span class="sxs-lookup"><span data-stu-id="142d2-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="142d2-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="142d2-125">JSON Representation</span></span>
<span data-ttu-id="142d2-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="142d2-126">Here is a JSON representation of the resource.</span></span>
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




