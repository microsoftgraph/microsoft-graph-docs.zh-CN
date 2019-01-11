---
title: bitLockerFixedDrivePolicy 资源类型
description: BitLocker 固定驱动器策略。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f55c2b81f1649c1292c4a54209480583147c9c23
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886938"
---
# <a name="bitlockerfixeddrivepolicy-resource-type"></a><span data-ttu-id="1b787-103">bitLockerFixedDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b787-103">bitLockerFixedDrivePolicy resource type</span></span>

> <span data-ttu-id="1b787-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1b787-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b787-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1b787-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b787-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1b787-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b787-107">BitLocker 固定驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="1b787-107">BitLocker Fixed Drive Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="1b787-108">属性</span><span class="sxs-lookup"><span data-stu-id="1b787-108">Properties</span></span>
|<span data-ttu-id="1b787-109">属性</span><span class="sxs-lookup"><span data-stu-id="1b787-109">Property</span></span>|<span data-ttu-id="1b787-110">类型</span><span class="sxs-lookup"><span data-stu-id="1b787-110">Type</span></span>|<span data-ttu-id="1b787-111">说明</span><span class="sxs-lookup"><span data-stu-id="1b787-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b787-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="1b787-112">encryptionMethod</span></span>|[<span data-ttu-id="1b787-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="1b787-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="1b787-114">选择固定驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="1b787-114">Select the encryption method for fixed drives.</span></span> <span data-ttu-id="1b787-115">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`</span><span class="sxs-lookup"><span data-stu-id="1b787-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="1b787-116">requireEncryptionForWriteAccess</span><span class="sxs-lookup"><span data-stu-id="1b787-116">requireEncryptionForWriteAccess</span></span>|<span data-ttu-id="1b787-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b787-117">Boolean</span></span>|<span data-ttu-id="1b787-118">此策略设置确定是否需要对固定的数据驱动器可写入的计算机上 BitLocker 保护。</span><span class="sxs-lookup"><span data-stu-id="1b787-118">This policy setting determines whether BitLocker protection is required for fixed data drives to be writable on a computer.</span></span>|
|<span data-ttu-id="1b787-119">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="1b787-119">recoveryOptions</span></span>|[<span data-ttu-id="1b787-120">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="1b787-120">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="1b787-121">此策略设置可以控制如何受保护的 BitLocker 驱动器恢复所需的凭据不存在的固定的数据。</span><span class="sxs-lookup"><span data-stu-id="1b787-121">This policy setting allows you to control how BitLocker-protected fixed data drives are recovered in the absence of the required credentials.</span></span> <span data-ttu-id="1b787-122">Bitlocker 打开时，将应用此策略设置。</span><span class="sxs-lookup"><span data-stu-id="1b787-122">This policy setting is applied when you turn on BitLocker.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b787-123">Relationships</span><span class="sxs-lookup"><span data-stu-id="1b787-123">Relationships</span></span>
<span data-ttu-id="1b787-124">无</span><span class="sxs-lookup"><span data-stu-id="1b787-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1b787-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b787-125">JSON Representation</span></span>
<span data-ttu-id="1b787-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b787-126">Here is a JSON representation of the resource.</span></span>
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





