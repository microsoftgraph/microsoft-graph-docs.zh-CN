---
title: bitLockerSystemDrivePolicy 资源类型
description: BitLocker 加密基本策略。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 82ed6d717c58f740dd25d2aff18478ced48c4641
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453671"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="e5b24-103">bitLockerSystemDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="e5b24-103">bitLockerSystemDrivePolicy resource type</span></span>

<span data-ttu-id="e5b24-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5b24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5b24-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e5b24-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5b24-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e5b24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5b24-107">BitLocker 加密基本策略。</span><span class="sxs-lookup"><span data-stu-id="e5b24-107">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="e5b24-108">属性</span><span class="sxs-lookup"><span data-stu-id="e5b24-108">Properties</span></span>
|<span data-ttu-id="e5b24-109">属性</span><span class="sxs-lookup"><span data-stu-id="e5b24-109">Property</span></span>|<span data-ttu-id="e5b24-110">类型</span><span class="sxs-lookup"><span data-stu-id="e5b24-110">Type</span></span>|<span data-ttu-id="e5b24-111">说明</span><span class="sxs-lookup"><span data-stu-id="e5b24-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5b24-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="e5b24-112">encryptionMethod</span></span>|[<span data-ttu-id="e5b24-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="e5b24-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="e5b24-114">选择操作系统驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="e5b24-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="e5b24-115">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`。</span><span class="sxs-lookup"><span data-stu-id="e5b24-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="e5b24-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="e5b24-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="e5b24-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b24-117">Boolean</span></span>|<span data-ttu-id="e5b24-118">启动时需要其他身份验证。</span><span class="sxs-lookup"><span data-stu-id="e5b24-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="e5b24-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="e5b24-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="e5b24-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b24-120">Boolean</span></span>|<span data-ttu-id="e5b24-121">指示是否允许没有兼容的 TPM 的 BitLocker （在 USB 闪存驱动器上需要密码或启动密钥）。</span><span class="sxs-lookup"><span data-stu-id="e5b24-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="e5b24-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="e5b24-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="e5b24-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="e5b24-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="e5b24-124">指示是否允许或不允许 TPM 启动。</span><span class="sxs-lookup"><span data-stu-id="e5b24-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="e5b24-125">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="e5b24-125">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="e5b24-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="e5b24-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="e5b24-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="e5b24-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="e5b24-128">指示是否允许或不允许 TPM 启动 pin。</span><span class="sxs-lookup"><span data-stu-id="e5b24-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="e5b24-129">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="e5b24-129">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="e5b24-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="e5b24-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="e5b24-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="e5b24-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="e5b24-132">指示是否允许或不允许 TPM 启动密钥。</span><span class="sxs-lookup"><span data-stu-id="e5b24-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="e5b24-133">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="e5b24-133">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="e5b24-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="e5b24-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="e5b24-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="e5b24-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="e5b24-136">指示是否允许/不允许使用 TPM 启动 pin 密钥和密钥。</span><span class="sxs-lookup"><span data-stu-id="e5b24-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="e5b24-137">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="e5b24-137">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="e5b24-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="e5b24-138">minimumPinLength</span></span>|<span data-ttu-id="e5b24-139">Int32</span><span class="sxs-lookup"><span data-stu-id="e5b24-139">Int32</span></span>|<span data-ttu-id="e5b24-140">指示启动 pin 的最小长度。</span><span class="sxs-lookup"><span data-stu-id="e5b24-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="e5b24-141">有效值为4至20</span><span class="sxs-lookup"><span data-stu-id="e5b24-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="e5b24-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="e5b24-142">recoveryOptions</span></span>|[<span data-ttu-id="e5b24-143">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="e5b24-143">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="e5b24-144">允许在缺少所需的启动密钥信息时恢复 BitLocker 加密的操作系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="e5b24-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="e5b24-145">启用 BitLocker 时，将应用此策略设置。</span><span class="sxs-lookup"><span data-stu-id="e5b24-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="e5b24-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="e5b24-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="e5b24-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5b24-147">Boolean</span></span>|<span data-ttu-id="e5b24-148">启用预引导恢复消息和 Url。</span><span class="sxs-lookup"><span data-stu-id="e5b24-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="e5b24-149">如果 requireStartupAuthentication 为 false，则此值不起作用。</span><span class="sxs-lookup"><span data-stu-id="e5b24-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="e5b24-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="e5b24-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="e5b24-151">String</span><span class="sxs-lookup"><span data-stu-id="e5b24-151">String</span></span>|<span data-ttu-id="e5b24-152">定义自定义恢复消息。</span><span class="sxs-lookup"><span data-stu-id="e5b24-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="e5b24-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="e5b24-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="e5b24-154">String</span><span class="sxs-lookup"><span data-stu-id="e5b24-154">String</span></span>|<span data-ttu-id="e5b24-155">定义自定义恢复 URL。</span><span class="sxs-lookup"><span data-stu-id="e5b24-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5b24-156">关系</span><span class="sxs-lookup"><span data-stu-id="e5b24-156">Relationships</span></span>
<span data-ttu-id="e5b24-157">无</span><span class="sxs-lookup"><span data-stu-id="e5b24-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5b24-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e5b24-158">JSON Representation</span></span>
<span data-ttu-id="e5b24-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e5b24-159">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": true,
  "startupAuthenticationBlockWithoutTpmChip": true,
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": 1024,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  },
  "prebootRecoveryEnableMessageAndUrl": true,
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```



