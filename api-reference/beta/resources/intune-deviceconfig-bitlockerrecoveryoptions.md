---
title: bitLockerRecoveryOptions 资源类型
description: BitLocker 恢复选项。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eae2052f71d1b1d048072c70dc76437811c1cd8f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806452"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="3150c-103">bitLockerRecoveryOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="3150c-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="3150c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3150c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3150c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3150c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3150c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3150c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3150c-107">BitLocker 恢复选项。</span><span class="sxs-lookup"><span data-stu-id="3150c-107">BitLocker Recovery Options.</span></span>
## <a name="properties"></a><span data-ttu-id="3150c-108">属性</span><span class="sxs-lookup"><span data-stu-id="3150c-108">Properties</span></span>
|<span data-ttu-id="3150c-109">属性</span><span class="sxs-lookup"><span data-stu-id="3150c-109">Property</span></span>|<span data-ttu-id="3150c-110">类型</span><span class="sxs-lookup"><span data-stu-id="3150c-110">Type</span></span>|<span data-ttu-id="3150c-111">Description</span><span class="sxs-lookup"><span data-stu-id="3150c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3150c-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="3150c-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="3150c-113">布尔</span><span class="sxs-lookup"><span data-stu-id="3150c-113">Boolean</span></span>|<span data-ttu-id="3150c-114">指示是否阻止基于证书的数据恢复代理。</span><span class="sxs-lookup"><span data-stu-id="3150c-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="3150c-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="3150c-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="3150c-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="3150c-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="3150c-117">指示是否允许用户或所需的固定生成 48 位数恢复密码或系统磁盘。</span><span class="sxs-lookup"><span data-stu-id="3150c-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="3150c-118">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="3150c-118">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="3150c-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="3150c-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="3150c-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="3150c-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="3150c-121">指示是否允许用户或所需的固定生成 256 位恢复密钥或系统磁盘。</span><span class="sxs-lookup"><span data-stu-id="3150c-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="3150c-122">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="3150c-122">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="3150c-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="3150c-123">hideRecoveryOptions</span></span>|<span data-ttu-id="3150c-124">布尔</span><span class="sxs-lookup"><span data-stu-id="3150c-124">Boolean</span></span>|<span data-ttu-id="3150c-125">指示允许在 BitLocker 安装向导中显示恢复选项的固定或系统磁盘。</span><span class="sxs-lookup"><span data-stu-id="3150c-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="3150c-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="3150c-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="3150c-127">布尔</span><span class="sxs-lookup"><span data-stu-id="3150c-127">Boolean</span></span>|<span data-ttu-id="3150c-128">指示允许 BitLocker 恢复信息将存储在 AD DS。</span><span class="sxs-lookup"><span data-stu-id="3150c-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="3150c-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="3150c-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="3150c-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="3150c-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="3150c-131">配置存储到 AD DS BitLocker 恢复信息的哪些部分。</span><span class="sxs-lookup"><span data-stu-id="3150c-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="3150c-132">可取值为：`passwordAndKey`、`passwordOnly`。</span><span class="sxs-lookup"><span data-stu-id="3150c-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="3150c-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="3150c-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="3150c-134">布尔</span><span class="sxs-lookup"><span data-stu-id="3150c-134">Boolean</span></span>|<span data-ttu-id="3150c-135">指示启用 BitLocker，直到恢复信息存储在 AD DS。</span><span class="sxs-lookup"><span data-stu-id="3150c-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3150c-136">Relationships</span><span class="sxs-lookup"><span data-stu-id="3150c-136">Relationships</span></span>
<span data-ttu-id="3150c-137">无</span><span class="sxs-lookup"><span data-stu-id="3150c-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3150c-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3150c-138">JSON Representation</span></span>
<span data-ttu-id="3150c-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3150c-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```





