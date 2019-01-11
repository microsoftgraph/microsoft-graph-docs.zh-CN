---
title: bitLockerSystemDrivePolicy 资源类型
description: BitLocker 加密的基本策略。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 030051faf1405cf15c138384c1b6ab8891fbae95
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867429"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="98541-103">bitLockerSystemDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="98541-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="98541-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="98541-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98541-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="98541-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98541-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="98541-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98541-107">BitLocker 加密的基本策略。</span><span class="sxs-lookup"><span data-stu-id="98541-107">BitLocker Encryption Base Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="98541-108">属性</span><span class="sxs-lookup"><span data-stu-id="98541-108">Properties</span></span>
|<span data-ttu-id="98541-109">属性</span><span class="sxs-lookup"><span data-stu-id="98541-109">Property</span></span>|<span data-ttu-id="98541-110">类型</span><span class="sxs-lookup"><span data-stu-id="98541-110">Type</span></span>|<span data-ttu-id="98541-111">说明</span><span class="sxs-lookup"><span data-stu-id="98541-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98541-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="98541-112">encryptionMethod</span></span>|[<span data-ttu-id="98541-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="98541-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="98541-114">选择操作系统驱动器的加密的方法。</span><span class="sxs-lookup"><span data-stu-id="98541-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="98541-115">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`。</span><span class="sxs-lookup"><span data-stu-id="98541-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="98541-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="98541-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="98541-117">布尔</span><span class="sxs-lookup"><span data-stu-id="98541-117">Boolean</span></span>|<span data-ttu-id="98541-118">需要在启动时的其他身份验证。</span><span class="sxs-lookup"><span data-stu-id="98541-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="98541-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="98541-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="98541-120">布尔</span><span class="sxs-lookup"><span data-stu-id="98541-120">Boolean</span></span>|<span data-ttu-id="98541-121">指示是否允许 BitLocker 不兼容的 TPM （需要密码或 USB 闪存驱动器上的启动项）。</span><span class="sxs-lookup"><span data-stu-id="98541-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="98541-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="98541-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="98541-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="98541-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="98541-124">指示是否允许使用或所需/禁止 TPM 启动。</span><span class="sxs-lookup"><span data-stu-id="98541-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="98541-125">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="98541-125">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="98541-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="98541-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="98541-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="98541-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="98541-128">指示是否允许使用或所需/禁止 TPM 启动 pin。</span><span class="sxs-lookup"><span data-stu-id="98541-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="98541-129">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="98541-129">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="98541-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="98541-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="98541-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="98541-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="98541-132">指示是否允许使用或所需/禁止 TPM 启动密钥。</span><span class="sxs-lookup"><span data-stu-id="98541-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="98541-133">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="98541-133">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="98541-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="98541-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="98541-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="98541-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="98541-136">指示是否 TPM 启动固定键和密钥是允许/所需/被禁止。</span><span class="sxs-lookup"><span data-stu-id="98541-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="98541-137">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="98541-137">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="98541-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="98541-138">minimumPinLength</span></span>|<span data-ttu-id="98541-139">Int32</span><span class="sxs-lookup"><span data-stu-id="98541-139">Int32</span></span>|<span data-ttu-id="98541-140">指示启动旋转中心点的最小长度。</span><span class="sxs-lookup"><span data-stu-id="98541-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="98541-141">有效值 4 到 20</span><span class="sxs-lookup"><span data-stu-id="98541-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="98541-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="98541-142">recoveryOptions</span></span>|[<span data-ttu-id="98541-143">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="98541-143">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="98541-144">允许恢复需要的启动关键信息不存在的 BitLocker 加密操作系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="98541-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="98541-145">Bitlocker 打开时，将应用此策略设置。</span><span class="sxs-lookup"><span data-stu-id="98541-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="98541-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="98541-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="98541-147">布尔</span><span class="sxs-lookup"><span data-stu-id="98541-147">Boolean</span></span>|<span data-ttu-id="98541-148">启用预启动恢复消息和 Url。</span><span class="sxs-lookup"><span data-stu-id="98541-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="98541-149">如果 requireStartupAuthentication 为 false，则不会影响此值。</span><span class="sxs-lookup"><span data-stu-id="98541-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="98541-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="98541-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="98541-151">字符串</span><span class="sxs-lookup"><span data-stu-id="98541-151">String</span></span>|<span data-ttu-id="98541-152">定义的自定义恢复消息。</span><span class="sxs-lookup"><span data-stu-id="98541-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="98541-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="98541-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="98541-154">字符串</span><span class="sxs-lookup"><span data-stu-id="98541-154">String</span></span>|<span data-ttu-id="98541-155">定义自定义恢复 URL。</span><span class="sxs-lookup"><span data-stu-id="98541-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98541-156">Relationships</span><span class="sxs-lookup"><span data-stu-id="98541-156">Relationships</span></span>
<span data-ttu-id="98541-157">无</span><span class="sxs-lookup"><span data-stu-id="98541-157">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98541-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98541-158">JSON Representation</span></span>
<span data-ttu-id="98541-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98541-159">Here is a JSON representation of the resource.</span></span>
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





