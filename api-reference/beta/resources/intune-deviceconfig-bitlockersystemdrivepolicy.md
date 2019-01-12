---
title: bitLockerSystemDrivePolicy 资源类型
description: BitLocker 加密的基本策略。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 28c3b597f25e7ea83577c18620280885f4149dcf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924655"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="ed0d3-103">bitLockerSystemDrivePolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed0d3-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="ed0d3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed0d3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed0d3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed0d3-107">BitLocker 加密的基本策略。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-107">BitLocker Encryption Base Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="ed0d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="ed0d3-108">Properties</span></span>
|<span data-ttu-id="ed0d3-109">属性</span><span class="sxs-lookup"><span data-stu-id="ed0d3-109">Property</span></span>|<span data-ttu-id="ed0d3-110">类型</span><span class="sxs-lookup"><span data-stu-id="ed0d3-110">Type</span></span>|<span data-ttu-id="ed0d3-111">说明</span><span class="sxs-lookup"><span data-stu-id="ed0d3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed0d3-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="ed0d3-112">encryptionMethod</span></span>|[<span data-ttu-id="ed0d3-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="ed0d3-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="ed0d3-114">选择操作系统驱动器的加密的方法。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="ed0d3-115">可取值为：`aesCbc128`、`aesCbc256`、`xtsAes128`、`xtsAes256`。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="ed0d3-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="ed0d3-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="ed0d3-117">布尔</span><span class="sxs-lookup"><span data-stu-id="ed0d3-117">Boolean</span></span>|<span data-ttu-id="ed0d3-118">需要在启动时的其他身份验证。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="ed0d3-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="ed0d3-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="ed0d3-120">布尔</span><span class="sxs-lookup"><span data-stu-id="ed0d3-120">Boolean</span></span>|<span data-ttu-id="ed0d3-121">指示是否允许 BitLocker 不兼容的 TPM （需要密码或 USB 闪存驱动器上的启动项）。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="ed0d3-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="ed0d3-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="ed0d3-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="ed0d3-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="ed0d3-124">指示是否允许使用或所需/禁止 TPM 启动。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="ed0d3-125">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-125">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="ed0d3-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="ed0d3-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="ed0d3-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="ed0d3-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="ed0d3-128">指示是否允许使用或所需/禁止 TPM 启动 pin。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="ed0d3-129">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-129">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="ed0d3-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="ed0d3-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="ed0d3-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="ed0d3-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="ed0d3-132">指示是否允许使用或所需/禁止 TPM 启动密钥。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="ed0d3-133">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-133">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="ed0d3-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="ed0d3-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="ed0d3-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="ed0d3-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="ed0d3-136">指示是否 TPM 启动固定键和密钥是允许/所需/被禁止。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="ed0d3-137">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-137">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="ed0d3-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="ed0d3-138">minimumPinLength</span></span>|<span data-ttu-id="ed0d3-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ed0d3-139">Int32</span></span>|<span data-ttu-id="ed0d3-140">指示启动旋转中心点的最小长度。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="ed0d3-141">有效值 4 到 20</span><span class="sxs-lookup"><span data-stu-id="ed0d3-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="ed0d3-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="ed0d3-142">recoveryOptions</span></span>|[<span data-ttu-id="ed0d3-143">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="ed0d3-143">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="ed0d3-144">允许恢复需要的启动关键信息不存在的 BitLocker 加密操作系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="ed0d3-145">Bitlocker 打开时，将应用此策略设置。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="ed0d3-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="ed0d3-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="ed0d3-147">布尔</span><span class="sxs-lookup"><span data-stu-id="ed0d3-147">Boolean</span></span>|<span data-ttu-id="ed0d3-148">启用预启动恢复消息和 Url。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="ed0d3-149">如果 requireStartupAuthentication 为 false，则不会影响此值。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="ed0d3-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="ed0d3-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="ed0d3-151">字符串</span><span class="sxs-lookup"><span data-stu-id="ed0d3-151">String</span></span>|<span data-ttu-id="ed0d3-152">定义的自定义恢复消息。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="ed0d3-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="ed0d3-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="ed0d3-154">字符串</span><span class="sxs-lookup"><span data-stu-id="ed0d3-154">String</span></span>|<span data-ttu-id="ed0d3-155">定义自定义恢复 URL。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed0d3-156">Relationships</span><span class="sxs-lookup"><span data-stu-id="ed0d3-156">Relationships</span></span>
<span data-ttu-id="ed0d3-157">无</span><span class="sxs-lookup"><span data-stu-id="ed0d3-157">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ed0d3-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed0d3-158">JSON Representation</span></span>
<span data-ttu-id="ed0d3-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed0d3-159">Here is a JSON representation of the resource.</span></span>
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





