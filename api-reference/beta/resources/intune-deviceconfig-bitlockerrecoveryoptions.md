---
title: bitLockerRecoveryOptions 资源类型
description: BitLocker 恢复选项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e9ac2b9fee5947de29cdf2d6cc4e56d521b9f131
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971072"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="83113-103">bitLockerRecoveryOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="83113-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="83113-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83113-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83113-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83113-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83113-106">BitLocker 恢复选项。</span><span class="sxs-lookup"><span data-stu-id="83113-106">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="83113-107">属性</span><span class="sxs-lookup"><span data-stu-id="83113-107">Properties</span></span>
|<span data-ttu-id="83113-108">属性</span><span class="sxs-lookup"><span data-stu-id="83113-108">Property</span></span>|<span data-ttu-id="83113-109">类型</span><span class="sxs-lookup"><span data-stu-id="83113-109">Type</span></span>|<span data-ttu-id="83113-110">说明</span><span class="sxs-lookup"><span data-stu-id="83113-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83113-111">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="83113-111">blockDataRecoveryAgent</span></span>|<span data-ttu-id="83113-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="83113-112">Boolean</span></span>|<span data-ttu-id="83113-113">指示是否阻止基于证书的数据恢复代理。</span><span class="sxs-lookup"><span data-stu-id="83113-113">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="83113-114">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="83113-114">recoveryPasswordUsage</span></span>|[<span data-ttu-id="83113-115">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="83113-115">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="83113-116">指示是否允许用户或需要用户为固定或系统磁盘生成48位数的恢复密码。</span><span class="sxs-lookup"><span data-stu-id="83113-116">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="83113-117">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="83113-117">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="83113-118">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="83113-118">recoveryKeyUsage</span></span>|[<span data-ttu-id="83113-119">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="83113-119">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="83113-120">指示是否允许用户或需要用户生成用于固定或系统磁盘的256位恢复密钥。</span><span class="sxs-lookup"><span data-stu-id="83113-120">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="83113-121">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="83113-121">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="83113-122">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="83113-122">hideRecoveryOptions</span></span>|<span data-ttu-id="83113-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="83113-123">Boolean</span></span>|<span data-ttu-id="83113-124">指示是否允许在 BitLocker 安装向导中显示固定或系统磁盘的恢复选项。</span><span class="sxs-lookup"><span data-stu-id="83113-124">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="83113-125">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="83113-125">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="83113-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="83113-126">Boolean</span></span>|<span data-ttu-id="83113-127">指示是否允许 BitLocker 恢复信息存储在 AD DS 中。</span><span class="sxs-lookup"><span data-stu-id="83113-127">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="83113-128">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="83113-128">recoveryInformationToStore</span></span>|[<span data-ttu-id="83113-129">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="83113-129">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="83113-130">配置存储在 AD DS 中的 BitLocker 恢复信息的哪些部分。</span><span class="sxs-lookup"><span data-stu-id="83113-130">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="83113-131">可取值为：`passwordAndKey`、`passwordOnly`。</span><span class="sxs-lookup"><span data-stu-id="83113-131">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="83113-132">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="83113-132">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="83113-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="83113-133">Boolean</span></span>|<span data-ttu-id="83113-134">指示在将恢复信息存储在 AD DS 中之前是否启用 BitLocker。</span><span class="sxs-lookup"><span data-stu-id="83113-134">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83113-135">关系</span><span class="sxs-lookup"><span data-stu-id="83113-135">Relationships</span></span>
<span data-ttu-id="83113-136">无</span><span class="sxs-lookup"><span data-stu-id="83113-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="83113-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83113-137">JSON Representation</span></span>
<span data-ttu-id="83113-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83113-138">Here is a JSON representation of the resource.</span></span>
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





