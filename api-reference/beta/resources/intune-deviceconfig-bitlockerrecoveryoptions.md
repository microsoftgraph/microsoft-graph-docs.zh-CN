---
title: bitLockerRecoveryOptions 资源类型
description: BitLocker 恢复选项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf88795ac9f2708bc03607bc5d48d5ec69a822eb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991049"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="7f6dc-103">bitLockerRecoveryOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f6dc-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="7f6dc-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f6dc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f6dc-106">BitLocker 恢复选项。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-106">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="7f6dc-107">属性</span><span class="sxs-lookup"><span data-stu-id="7f6dc-107">Properties</span></span>
|<span data-ttu-id="7f6dc-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f6dc-108">Property</span></span>|<span data-ttu-id="7f6dc-109">类型</span><span class="sxs-lookup"><span data-stu-id="7f6dc-109">Type</span></span>|<span data-ttu-id="7f6dc-110">说明</span><span class="sxs-lookup"><span data-stu-id="7f6dc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f6dc-111">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="7f6dc-111">blockDataRecoveryAgent</span></span>|<span data-ttu-id="7f6dc-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f6dc-112">Boolean</span></span>|<span data-ttu-id="7f6dc-113">指示是否阻止基于证书的数据恢复代理。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-113">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="7f6dc-114">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="7f6dc-114">recoveryPasswordUsage</span></span>|[<span data-ttu-id="7f6dc-115">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="7f6dc-115">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="7f6dc-116">指示是否允许用户或需要用户为固定或系统磁盘生成48位数的恢复密码。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-116">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="7f6dc-117">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-117">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="7f6dc-118">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="7f6dc-118">recoveryKeyUsage</span></span>|[<span data-ttu-id="7f6dc-119">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="7f6dc-119">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="7f6dc-120">指示是否允许用户或需要用户生成用于固定或系统磁盘的256位恢复密钥。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-120">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="7f6dc-121">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-121">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="7f6dc-122">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="7f6dc-122">hideRecoveryOptions</span></span>|<span data-ttu-id="7f6dc-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f6dc-123">Boolean</span></span>|<span data-ttu-id="7f6dc-124">指示是否允许在 BitLocker 安装向导中显示固定或系统磁盘的恢复选项。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-124">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="7f6dc-125">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="7f6dc-125">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="7f6dc-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f6dc-126">Boolean</span></span>|<span data-ttu-id="7f6dc-127">指示是否允许 BitLocker 恢复信息存储在 AD DS 中。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-127">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="7f6dc-128">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="7f6dc-128">recoveryInformationToStore</span></span>|[<span data-ttu-id="7f6dc-129">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="7f6dc-129">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="7f6dc-130">配置存储在 AD DS 中的 BitLocker 恢复信息的哪些部分。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-130">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="7f6dc-131">可取值为：`passwordAndKey`、`passwordOnly`。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-131">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="7f6dc-132">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="7f6dc-132">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="7f6dc-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f6dc-133">Boolean</span></span>|<span data-ttu-id="7f6dc-134">指示在将恢复信息存储在 AD DS 中之前是否启用 BitLocker。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-134">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f6dc-135">关系</span><span class="sxs-lookup"><span data-stu-id="7f6dc-135">Relationships</span></span>
<span data-ttu-id="7f6dc-136">无</span><span class="sxs-lookup"><span data-stu-id="7f6dc-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f6dc-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f6dc-137">JSON Representation</span></span>
<span data-ttu-id="7f6dc-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f6dc-138">Here is a JSON representation of the resource.</span></span>
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





