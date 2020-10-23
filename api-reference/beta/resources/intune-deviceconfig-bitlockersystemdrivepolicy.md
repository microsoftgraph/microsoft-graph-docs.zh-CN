---
title: bitLockerSystemDrivePolicy 资源类型
description: BitLocker 加密基本策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 16b03a021349e872451e22561305f7f79bf8b438
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729831"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="9976e-103">bitLockerSystemDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="9976e-103">bitLockerSystemDrivePolicy resource type</span></span>

<span data-ttu-id="9976e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9976e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9976e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9976e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9976e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9976e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9976e-107">BitLocker 加密基本策略。</span><span class="sxs-lookup"><span data-stu-id="9976e-107">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="9976e-108">属性</span><span class="sxs-lookup"><span data-stu-id="9976e-108">Properties</span></span>
|<span data-ttu-id="9976e-109">属性</span><span class="sxs-lookup"><span data-stu-id="9976e-109">Property</span></span>|<span data-ttu-id="9976e-110">类型</span><span class="sxs-lookup"><span data-stu-id="9976e-110">Type</span></span>|<span data-ttu-id="9976e-111">说明</span><span class="sxs-lookup"><span data-stu-id="9976e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9976e-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="9976e-112">encryptionMethod</span></span>|[<span data-ttu-id="9976e-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="9976e-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="9976e-114">选择操作系统驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="9976e-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="9976e-115">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`。</span><span class="sxs-lookup"><span data-stu-id="9976e-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="9976e-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="9976e-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="9976e-117">布尔</span><span class="sxs-lookup"><span data-stu-id="9976e-117">Boolean</span></span>|<span data-ttu-id="9976e-118">启动时需要其他身份验证。</span><span class="sxs-lookup"><span data-stu-id="9976e-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="9976e-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="9976e-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="9976e-120">布尔</span><span class="sxs-lookup"><span data-stu-id="9976e-120">Boolean</span></span>|<span data-ttu-id="9976e-121">指示是否允许没有兼容的 TPM (的 BitLocker 在 USB 闪存驱动器) 上需要密码或启动密钥。</span><span class="sxs-lookup"><span data-stu-id="9976e-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="9976e-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="9976e-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="9976e-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="9976e-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="9976e-124">指示是否允许或不允许 TPM 启动。</span><span class="sxs-lookup"><span data-stu-id="9976e-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="9976e-125">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="9976e-125">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="9976e-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="9976e-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="9976e-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="9976e-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="9976e-128">指示是否允许或不允许 TPM 启动 pin。</span><span class="sxs-lookup"><span data-stu-id="9976e-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="9976e-129">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="9976e-129">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="9976e-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="9976e-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="9976e-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="9976e-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="9976e-132">指示是否允许或不允许 TPM 启动密钥。</span><span class="sxs-lookup"><span data-stu-id="9976e-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="9976e-133">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="9976e-133">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="9976e-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="9976e-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="9976e-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="9976e-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="9976e-136">指示是否允许/不允许使用 TPM 启动 pin 密钥和密钥。</span><span class="sxs-lookup"><span data-stu-id="9976e-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="9976e-137">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="9976e-137">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="9976e-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="9976e-138">minimumPinLength</span></span>|<span data-ttu-id="9976e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="9976e-139">Int32</span></span>|<span data-ttu-id="9976e-140">指示启动 pin 的最小长度。</span><span class="sxs-lookup"><span data-stu-id="9976e-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="9976e-141">有效值为4至20</span><span class="sxs-lookup"><span data-stu-id="9976e-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="9976e-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="9976e-142">recoveryOptions</span></span>|[<span data-ttu-id="9976e-143">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="9976e-143">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="9976e-144">允许在缺少所需的启动密钥信息时恢复 BitLocker 加密的操作系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="9976e-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="9976e-145">启用 BitLocker 时，将应用此策略设置。</span><span class="sxs-lookup"><span data-stu-id="9976e-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="9976e-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="9976e-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="9976e-147">布尔</span><span class="sxs-lookup"><span data-stu-id="9976e-147">Boolean</span></span>|<span data-ttu-id="9976e-148">启用预引导恢复消息和 Url。</span><span class="sxs-lookup"><span data-stu-id="9976e-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="9976e-149">如果 requireStartupAuthentication 为 false，则此值不起作用。</span><span class="sxs-lookup"><span data-stu-id="9976e-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="9976e-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="9976e-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="9976e-151">String</span><span class="sxs-lookup"><span data-stu-id="9976e-151">String</span></span>|<span data-ttu-id="9976e-152">定义自定义恢复消息。</span><span class="sxs-lookup"><span data-stu-id="9976e-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="9976e-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="9976e-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="9976e-154">String</span><span class="sxs-lookup"><span data-stu-id="9976e-154">String</span></span>|<span data-ttu-id="9976e-155">定义自定义恢复 URL。</span><span class="sxs-lookup"><span data-stu-id="9976e-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9976e-156">关系</span><span class="sxs-lookup"><span data-stu-id="9976e-156">Relationships</span></span>
<span data-ttu-id="9976e-157">无</span><span class="sxs-lookup"><span data-stu-id="9976e-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9976e-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9976e-158">JSON Representation</span></span>
<span data-ttu-id="9976e-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9976e-159">Here is a JSON representation of the resource.</span></span>
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





