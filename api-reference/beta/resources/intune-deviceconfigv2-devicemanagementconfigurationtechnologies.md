---
title: deviceManagementConfigurationTechnologies 枚举类型
description: 描述可以使用哪种技术部署此设置
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b0e6a6324f9157fb528fd5aeb7772f4c1e8721fe
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666693"
---
# <a name="devicemanagementconfigurationtechnologies-enum-type"></a><span data-ttu-id="002aa-103">deviceManagementConfigurationTechnologies 枚举类型</span><span class="sxs-lookup"><span data-stu-id="002aa-103">deviceManagementConfigurationTechnologies enum type</span></span>

<span data-ttu-id="002aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="002aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="002aa-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="002aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="002aa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="002aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="002aa-107">描述可以使用哪种技术部署此设置</span><span class="sxs-lookup"><span data-stu-id="002aa-107">Describes which technology this setting can be deployed with</span></span>

## <a name="members"></a><span data-ttu-id="002aa-108">成员</span><span class="sxs-lookup"><span data-stu-id="002aa-108">Members</span></span>
|<span data-ttu-id="002aa-109">成员</span><span class="sxs-lookup"><span data-stu-id="002aa-109">Member</span></span>|<span data-ttu-id="002aa-110">值</span><span class="sxs-lookup"><span data-stu-id="002aa-110">Value</span></span>|<span data-ttu-id="002aa-111">说明</span><span class="sxs-lookup"><span data-stu-id="002aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="002aa-112">无</span><span class="sxs-lookup"><span data-stu-id="002aa-112">none</span></span>|<span data-ttu-id="002aa-113">0</span><span class="sxs-lookup"><span data-stu-id="002aa-113">0</span></span>|<span data-ttu-id="002aa-114">无法通过任何通道部署设置</span><span class="sxs-lookup"><span data-stu-id="002aa-114">Setting cannot be deployed through any channel</span></span>|
|<span data-ttu-id="002aa-115">mdm</span><span class="sxs-lookup"><span data-stu-id="002aa-115">mdm</span></span>|<span data-ttu-id="002aa-116">1</span><span class="sxs-lookup"><span data-stu-id="002aa-116">1</span></span>|<span data-ttu-id="002aa-117">可通过 MDM 通道部署设置</span><span class="sxs-lookup"><span data-stu-id="002aa-117">Setting can be deployed through the MDM channel</span></span>|
|<span data-ttu-id="002aa-118">windows10XManagement</span><span class="sxs-lookup"><span data-stu-id="002aa-118">windows10XManagement</span></span>|<span data-ttu-id="002aa-119">2</span><span class="sxs-lookup"><span data-stu-id="002aa-119">2</span></span>|<span data-ttu-id="002aa-120">可通过 Windows10XManagement 通道部署设置</span><span class="sxs-lookup"><span data-stu-id="002aa-120">Setting can be deployed through the Windows10XManagement channel</span></span>|
|<span data-ttu-id="002aa-121">configManager</span><span class="sxs-lookup"><span data-stu-id="002aa-121">configManager</span></span>|<span data-ttu-id="002aa-122">4 </span><span class="sxs-lookup"><span data-stu-id="002aa-122">4</span></span>|<span data-ttu-id="002aa-123">可通过 ConfigManager 通道部署设置</span><span class="sxs-lookup"><span data-stu-id="002aa-123">Setting can be deployed through the ConfigManager channel</span></span>|
|<span data-ttu-id="002aa-124">microsoftSense</span><span class="sxs-lookup"><span data-stu-id="002aa-124">microsoftSense</span></span>|<span data-ttu-id="002aa-125">128</span><span class="sxs-lookup"><span data-stu-id="002aa-125">128</span></span>|<span data-ttu-id="002aa-126">可以通过 SENSE 代理通道部署设置</span><span class="sxs-lookup"><span data-stu-id="002aa-126">Setting can be deployed through the SENSE agent channel</span></span>|




