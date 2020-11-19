---
title: bitLockerSystemDrivePolicy 资源类型
description: BitLocker 加密基本策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 605236c0f1a1a1f5a4aea3554ff118aebaac15f7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260521"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="23a07-103">bitLockerSystemDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="23a07-103">bitLockerSystemDrivePolicy resource type</span></span>

<span data-ttu-id="23a07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23a07-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23a07-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23a07-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23a07-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23a07-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23a07-107">BitLocker 加密基本策略。</span><span class="sxs-lookup"><span data-stu-id="23a07-107">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="23a07-108">属性</span><span class="sxs-lookup"><span data-stu-id="23a07-108">Properties</span></span>
|<span data-ttu-id="23a07-109">属性</span><span class="sxs-lookup"><span data-stu-id="23a07-109">Property</span></span>|<span data-ttu-id="23a07-110">类型</span><span class="sxs-lookup"><span data-stu-id="23a07-110">Type</span></span>|<span data-ttu-id="23a07-111">描述</span><span class="sxs-lookup"><span data-stu-id="23a07-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23a07-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="23a07-112">encryptionMethod</span></span>|[<span data-ttu-id="23a07-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="23a07-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="23a07-114">选择操作系统驱动器的加密方法。</span><span class="sxs-lookup"><span data-stu-id="23a07-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="23a07-115">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`。</span><span class="sxs-lookup"><span data-stu-id="23a07-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="23a07-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="23a07-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="23a07-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="23a07-117">Boolean</span></span>|<span data-ttu-id="23a07-118">启动时需要其他身份验证。</span><span class="sxs-lookup"><span data-stu-id="23a07-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="23a07-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="23a07-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="23a07-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="23a07-120">Boolean</span></span>|<span data-ttu-id="23a07-121">指示是否允许没有兼容的 TPM (的 BitLocker 在 USB 闪存驱动器) 上需要密码或启动密钥。</span><span class="sxs-lookup"><span data-stu-id="23a07-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="23a07-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="23a07-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="23a07-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="23a07-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="23a07-124">指示是否允许或不允许 TPM 启动。</span><span class="sxs-lookup"><span data-stu-id="23a07-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="23a07-125">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="23a07-125">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="23a07-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="23a07-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="23a07-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="23a07-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="23a07-128">指示是否允许或不允许 TPM 启动 pin。</span><span class="sxs-lookup"><span data-stu-id="23a07-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="23a07-129">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="23a07-129">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="23a07-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="23a07-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="23a07-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="23a07-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="23a07-132">指示是否允许或不允许 TPM 启动密钥。</span><span class="sxs-lookup"><span data-stu-id="23a07-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="23a07-133">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="23a07-133">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="23a07-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="23a07-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="23a07-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="23a07-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="23a07-136">指示是否允许/不允许使用 TPM 启动 pin 密钥和密钥。</span><span class="sxs-lookup"><span data-stu-id="23a07-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="23a07-137">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="23a07-137">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="23a07-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="23a07-138">minimumPinLength</span></span>|<span data-ttu-id="23a07-139">Int32</span><span class="sxs-lookup"><span data-stu-id="23a07-139">Int32</span></span>|<span data-ttu-id="23a07-140">指示启动 pin 的最小长度。</span><span class="sxs-lookup"><span data-stu-id="23a07-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="23a07-141">有效值为4至20</span><span class="sxs-lookup"><span data-stu-id="23a07-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="23a07-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="23a07-142">recoveryOptions</span></span>|[<span data-ttu-id="23a07-143">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="23a07-143">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="23a07-144">允许在缺少所需的启动密钥信息时恢复 BitLocker 加密的操作系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="23a07-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="23a07-145">启用 BitLocker 时，将应用此策略设置。</span><span class="sxs-lookup"><span data-stu-id="23a07-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="23a07-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="23a07-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="23a07-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="23a07-147">Boolean</span></span>|<span data-ttu-id="23a07-148">启用预引导恢复消息和 Url。</span><span class="sxs-lookup"><span data-stu-id="23a07-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="23a07-149">如果 requireStartupAuthentication 为 false，则此值不起作用。</span><span class="sxs-lookup"><span data-stu-id="23a07-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="23a07-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="23a07-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="23a07-151">String</span><span class="sxs-lookup"><span data-stu-id="23a07-151">String</span></span>|<span data-ttu-id="23a07-152">定义自定义恢复消息。</span><span class="sxs-lookup"><span data-stu-id="23a07-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="23a07-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="23a07-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="23a07-154">String</span><span class="sxs-lookup"><span data-stu-id="23a07-154">String</span></span>|<span data-ttu-id="23a07-155">定义自定义恢复 URL。</span><span class="sxs-lookup"><span data-stu-id="23a07-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23a07-156">关系</span><span class="sxs-lookup"><span data-stu-id="23a07-156">Relationships</span></span>
<span data-ttu-id="23a07-157">无</span><span class="sxs-lookup"><span data-stu-id="23a07-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23a07-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23a07-158">JSON Representation</span></span>
<span data-ttu-id="23a07-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23a07-159">Here is a JSON representation of the resource.</span></span>
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




