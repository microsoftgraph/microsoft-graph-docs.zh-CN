---
title: bitLockerRecoveryOptions 资源类型
description: BitLocker 恢复选项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 554cbe66021755755b3b181d0601e0007f525ba8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075796"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="baeac-103">bitLockerRecoveryOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="baeac-103">bitLockerRecoveryOptions resource type</span></span>

<span data-ttu-id="baeac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="baeac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="baeac-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="baeac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="baeac-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="baeac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baeac-107">BitLocker 恢复选项。</span><span class="sxs-lookup"><span data-stu-id="baeac-107">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="baeac-108">属性</span><span class="sxs-lookup"><span data-stu-id="baeac-108">Properties</span></span>
|<span data-ttu-id="baeac-109">属性</span><span class="sxs-lookup"><span data-stu-id="baeac-109">Property</span></span>|<span data-ttu-id="baeac-110">类型</span><span class="sxs-lookup"><span data-stu-id="baeac-110">Type</span></span>|<span data-ttu-id="baeac-111">说明</span><span class="sxs-lookup"><span data-stu-id="baeac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baeac-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="baeac-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="baeac-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="baeac-113">Boolean</span></span>|<span data-ttu-id="baeac-114">指示是否阻止基于证书的数据恢复代理。</span><span class="sxs-lookup"><span data-stu-id="baeac-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="baeac-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="baeac-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="baeac-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="baeac-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="baeac-117">指示是否允许用户或需要用户为固定或系统磁盘生成48位数的恢复密码。</span><span class="sxs-lookup"><span data-stu-id="baeac-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="baeac-118">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="baeac-118">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="baeac-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="baeac-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="baeac-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="baeac-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="baeac-121">指示是否允许用户或需要用户生成用于固定或系统磁盘的256位恢复密钥。</span><span class="sxs-lookup"><span data-stu-id="baeac-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="baeac-122">可取值为：`blocked`、`required`、`allowed`、`notConfigured`。</span><span class="sxs-lookup"><span data-stu-id="baeac-122">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="baeac-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="baeac-123">hideRecoveryOptions</span></span>|<span data-ttu-id="baeac-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="baeac-124">Boolean</span></span>|<span data-ttu-id="baeac-125">指示是否允许在 BitLocker 安装向导中显示固定或系统磁盘的恢复选项。</span><span class="sxs-lookup"><span data-stu-id="baeac-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="baeac-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="baeac-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="baeac-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="baeac-127">Boolean</span></span>|<span data-ttu-id="baeac-128">指示是否允许 BitLocker 恢复信息存储在 AD DS 中。</span><span class="sxs-lookup"><span data-stu-id="baeac-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="baeac-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="baeac-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="baeac-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="baeac-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="baeac-131">配置存储在 AD DS 中的 BitLocker 恢复信息的哪些部分。</span><span class="sxs-lookup"><span data-stu-id="baeac-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="baeac-132">可取值为：`passwordAndKey`、`passwordOnly`。</span><span class="sxs-lookup"><span data-stu-id="baeac-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="baeac-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="baeac-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="baeac-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="baeac-134">Boolean</span></span>|<span data-ttu-id="baeac-135">指示在将恢复信息存储在 AD DS 中之前是否启用 BitLocker。</span><span class="sxs-lookup"><span data-stu-id="baeac-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="baeac-136">关系</span><span class="sxs-lookup"><span data-stu-id="baeac-136">Relationships</span></span>
<span data-ttu-id="baeac-137">无</span><span class="sxs-lookup"><span data-stu-id="baeac-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="baeac-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="baeac-138">JSON Representation</span></span>
<span data-ttu-id="baeac-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="baeac-139">Here is a JSON representation of the resource.</span></span>
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






