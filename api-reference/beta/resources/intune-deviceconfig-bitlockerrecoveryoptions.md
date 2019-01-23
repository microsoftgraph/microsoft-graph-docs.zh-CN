---
title: bitLockerRecoveryOptions 资源类型
description: BitLocker 恢复选项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df1a2d0a9be3f4ec52b5fa289d0315bda36e4a59
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398511"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="73561-103">bitLockerRecoveryOptions 资源类型</span><span class="sxs-lookup"><span data-stu-id="73561-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="73561-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="73561-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="73561-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="73561-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73561-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73561-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73561-107">BitLocker 恢复选项。</span><span class="sxs-lookup"><span data-stu-id="73561-107">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="73561-108">属性</span><span class="sxs-lookup"><span data-stu-id="73561-108">Properties</span></span>
|<span data-ttu-id="73561-109">属性</span><span class="sxs-lookup"><span data-stu-id="73561-109">Property</span></span>|<span data-ttu-id="73561-110">类型</span><span class="sxs-lookup"><span data-stu-id="73561-110">Type</span></span>|<span data-ttu-id="73561-111">说明</span><span class="sxs-lookup"><span data-stu-id="73561-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73561-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="73561-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="73561-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="73561-113">Boolean</span></span>|<span data-ttu-id="73561-114">指示是否阻止基于证书的数据恢复代理。</span><span class="sxs-lookup"><span data-stu-id="73561-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="73561-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="73561-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="73561-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="73561-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="73561-117">指示是否允许用户或所需的固定生成 48 位数恢复密码或系统磁盘。</span><span class="sxs-lookup"><span data-stu-id="73561-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="73561-118">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="73561-118">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="73561-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="73561-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="73561-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="73561-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="73561-121">指示是否允许用户或所需的固定生成 256 位恢复密钥或系统磁盘。</span><span class="sxs-lookup"><span data-stu-id="73561-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="73561-122">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="73561-122">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="73561-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="73561-123">hideRecoveryOptions</span></span>|<span data-ttu-id="73561-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="73561-124">Boolean</span></span>|<span data-ttu-id="73561-125">指示允许在 BitLocker 安装向导中显示恢复选项的固定或系统磁盘。</span><span class="sxs-lookup"><span data-stu-id="73561-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="73561-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="73561-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="73561-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="73561-127">Boolean</span></span>|<span data-ttu-id="73561-128">指示允许 BitLocker 恢复信息将存储在 AD DS。</span><span class="sxs-lookup"><span data-stu-id="73561-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="73561-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="73561-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="73561-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="73561-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="73561-131">配置存储到 AD DS BitLocker 恢复信息的哪些部分。</span><span class="sxs-lookup"><span data-stu-id="73561-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="73561-132">可取值为：`passwordAndKey`、`passwordOnly`。</span><span class="sxs-lookup"><span data-stu-id="73561-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="73561-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="73561-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="73561-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="73561-134">Boolean</span></span>|<span data-ttu-id="73561-135">指示启用 BitLocker，直到恢复信息存储在 AD DS。</span><span class="sxs-lookup"><span data-stu-id="73561-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="73561-136">关系</span><span class="sxs-lookup"><span data-stu-id="73561-136">Relationships</span></span>
<span data-ttu-id="73561-137">无</span><span class="sxs-lookup"><span data-stu-id="73561-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="73561-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73561-138">JSON Representation</span></span>
<span data-ttu-id="73561-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73561-139">Here is a JSON representation of the resource.</span></span>
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




