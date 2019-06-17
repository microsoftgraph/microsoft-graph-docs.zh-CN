---
title: bitLockerSystemDrivePolicy 资源类型
description: BitLocker 加密基本策略。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bca77059f2ec819f62326469454f373b3916b7f7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990181"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="3da51-103">bitLockerSystemDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="3da51-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="3da51-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3da51-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3da51-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3da51-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3da51-106">BitLocker 加密基本策略。</span><span class="sxs-lookup"><span data-stu-id="3da51-106">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="3da51-107">属性</span><span class="sxs-lookup"><span data-stu-id="3da51-107">Properties</span></span>
|<span data-ttu-id="3da51-108">属性</span><span class="sxs-lookup"><span data-stu-id="3da51-108">Property</span></span>|<span data-ttu-id="3da51-109">类型</span><span class="sxs-lookup"><span data-stu-id="3da51-109">Type</span></span>|<span data-ttu-id="3da51-110">说明</span><span class="sxs-lookup"><span data-stu-id="3da51-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3da51-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="3da51-111">encryptionMethod</span></span>|[<span data-ttu-id="3da51-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="3da51-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="3da51-113">选择操作系统驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="3da51-113">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="3da51-114">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`。</span><span class="sxs-lookup"><span data-stu-id="3da51-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="3da51-115">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="3da51-115">startupAuthenticationRequired</span></span>|<span data-ttu-id="3da51-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="3da51-116">Boolean</span></span>|<span data-ttu-id="3da51-117">启动时需要其他身份验证。</span><span class="sxs-lookup"><span data-stu-id="3da51-117">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="3da51-118">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="3da51-118">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="3da51-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="3da51-119">Boolean</span></span>|<span data-ttu-id="3da51-120">指示是否允许没有兼容的 TPM 的 BitLocker (在 USB 闪存驱动器上需要密码或启动密钥)。</span><span class="sxs-lookup"><span data-stu-id="3da51-120">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="3da51-121">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="3da51-121">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="3da51-122">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="3da51-122">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="3da51-123">指示是否允许或不允许 TPM 启动。</span><span class="sxs-lookup"><span data-stu-id="3da51-123">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="3da51-124">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="3da51-124">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="3da51-125">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="3da51-125">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="3da51-126">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="3da51-126">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="3da51-127">指示是否允许或不允许 TPM 启动 pin。</span><span class="sxs-lookup"><span data-stu-id="3da51-127">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="3da51-128">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="3da51-128">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="3da51-129">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="3da51-129">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="3da51-130">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="3da51-130">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="3da51-131">指示是否允许或不允许 TPM 启动密钥。</span><span class="sxs-lookup"><span data-stu-id="3da51-131">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="3da51-132">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="3da51-132">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="3da51-133">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="3da51-133">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="3da51-134">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="3da51-134">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="3da51-135">指示是否允许/不允许使用 TPM 启动 pin 密钥和密钥。</span><span class="sxs-lookup"><span data-stu-id="3da51-135">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="3da51-136">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="3da51-136">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="3da51-137">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="3da51-137">minimumPinLength</span></span>|<span data-ttu-id="3da51-138">Int32</span><span class="sxs-lookup"><span data-stu-id="3da51-138">Int32</span></span>|<span data-ttu-id="3da51-139">指示启动 pin 的最小长度。</span><span class="sxs-lookup"><span data-stu-id="3da51-139">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="3da51-140">有效值为4至20</span><span class="sxs-lookup"><span data-stu-id="3da51-140">Valid values 4 to 20</span></span>|
|<span data-ttu-id="3da51-141">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="3da51-141">recoveryOptions</span></span>|[<span data-ttu-id="3da51-142">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="3da51-142">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="3da51-143">允许在缺少所需的启动密钥信息时恢复 BitLocker 加密的操作系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="3da51-143">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="3da51-144">启用 BitLocker 时, 将应用此策略设置。</span><span class="sxs-lookup"><span data-stu-id="3da51-144">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="3da51-145">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="3da51-145">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="3da51-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="3da51-146">Boolean</span></span>|<span data-ttu-id="3da51-147">启用预引导恢复消息和 Url。</span><span class="sxs-lookup"><span data-stu-id="3da51-147">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="3da51-148">如果 requireStartupAuthentication 为 false, 则此值不起作用。</span><span class="sxs-lookup"><span data-stu-id="3da51-148">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="3da51-149">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="3da51-149">prebootRecoveryMessage</span></span>|<span data-ttu-id="3da51-150">String</span><span class="sxs-lookup"><span data-stu-id="3da51-150">String</span></span>|<span data-ttu-id="3da51-151">定义自定义恢复消息。</span><span class="sxs-lookup"><span data-stu-id="3da51-151">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="3da51-152">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="3da51-152">prebootRecoveryUrl</span></span>|<span data-ttu-id="3da51-153">String</span><span class="sxs-lookup"><span data-stu-id="3da51-153">String</span></span>|<span data-ttu-id="3da51-154">定义自定义恢复 URL。</span><span class="sxs-lookup"><span data-stu-id="3da51-154">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3da51-155">关系</span><span class="sxs-lookup"><span data-stu-id="3da51-155">Relationships</span></span>
<span data-ttu-id="3da51-156">无</span><span class="sxs-lookup"><span data-stu-id="3da51-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3da51-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3da51-157">JSON Representation</span></span>
<span data-ttu-id="3da51-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3da51-158">Here is a JSON representation of the resource.</span></span>
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





