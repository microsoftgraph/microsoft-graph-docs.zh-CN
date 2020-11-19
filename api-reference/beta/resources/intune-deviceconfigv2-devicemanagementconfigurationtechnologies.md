---
title: deviceManagementConfigurationTechnologies 枚举类型
description: 介绍此设置可以部署到哪种技术
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8541d689fc18933a98c916ed004927094e4af0f9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49336981"
---
# <a name="devicemanagementconfigurationtechnologies-enum-type"></a><span data-ttu-id="97f52-103">deviceManagementConfigurationTechnologies 枚举类型</span><span class="sxs-lookup"><span data-stu-id="97f52-103">deviceManagementConfigurationTechnologies enum type</span></span>

<span data-ttu-id="97f52-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97f52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="97f52-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="97f52-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97f52-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97f52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97f52-107">介绍此设置可以部署到哪种技术</span><span class="sxs-lookup"><span data-stu-id="97f52-107">Describes which technology this setting can be deployed with</span></span>

## <a name="members"></a><span data-ttu-id="97f52-108">成员</span><span class="sxs-lookup"><span data-stu-id="97f52-108">Members</span></span>
|<span data-ttu-id="97f52-109">成员</span><span class="sxs-lookup"><span data-stu-id="97f52-109">Member</span></span>|<span data-ttu-id="97f52-110">值</span><span class="sxs-lookup"><span data-stu-id="97f52-110">Value</span></span>|<span data-ttu-id="97f52-111">Description</span><span class="sxs-lookup"><span data-stu-id="97f52-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97f52-112">无</span><span class="sxs-lookup"><span data-stu-id="97f52-112">none</span></span>|<span data-ttu-id="97f52-113">0</span><span class="sxs-lookup"><span data-stu-id="97f52-113">0</span></span>|<span data-ttu-id="97f52-114">无法通过任何通道部署设置</span><span class="sxs-lookup"><span data-stu-id="97f52-114">Setting cannot be deployed through any channel</span></span>|
|<span data-ttu-id="97f52-115">mdm</span><span class="sxs-lookup"><span data-stu-id="97f52-115">mdm</span></span>|<span data-ttu-id="97f52-116">1</span><span class="sxs-lookup"><span data-stu-id="97f52-116">1</span></span>|<span data-ttu-id="97f52-117">可以通过 MDM 通道部署设置</span><span class="sxs-lookup"><span data-stu-id="97f52-117">Setting can be deployed through the MDM channel</span></span>|
|<span data-ttu-id="97f52-118">windows10XManagement</span><span class="sxs-lookup"><span data-stu-id="97f52-118">windows10XManagement</span></span>|<span data-ttu-id="97f52-119">双面</span><span class="sxs-lookup"><span data-stu-id="97f52-119">2</span></span>|<span data-ttu-id="97f52-120">可以通过 Windows10XManagement 通道部署设置</span><span class="sxs-lookup"><span data-stu-id="97f52-120">Setting can be deployed through the Windows10XManagement channel</span></span>|
|<span data-ttu-id="97f52-121">configManager</span><span class="sxs-lookup"><span data-stu-id="97f52-121">configManager</span></span>|<span data-ttu-id="97f52-122">4 </span><span class="sxs-lookup"><span data-stu-id="97f52-122">4</span></span>|<span data-ttu-id="97f52-123">可以通过 ConfigManager 通道部署设置</span><span class="sxs-lookup"><span data-stu-id="97f52-123">Setting can be deployed through the ConfigManager channel</span></span>|




