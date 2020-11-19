---
title: windowsPrivacyDataAccessLevel 枚举类型
description: 确定特定 Windows 隐私数据类别的访问级别。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: acd71682d7e682dec53bb87885374aabdd38089d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215189"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="24988-103">windowsPrivacyDataAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="24988-103">windowsPrivacyDataAccessLevel enum type</span></span>

<span data-ttu-id="24988-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24988-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24988-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24988-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24988-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24988-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24988-107">确定特定 Windows 隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="24988-107">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="24988-108">成员</span><span class="sxs-lookup"><span data-stu-id="24988-108">Members</span></span>
|<span data-ttu-id="24988-109">成员</span><span class="sxs-lookup"><span data-stu-id="24988-109">Member</span></span>|<span data-ttu-id="24988-110">值</span><span class="sxs-lookup"><span data-stu-id="24988-110">Value</span></span>|<span data-ttu-id="24988-111">说明</span><span class="sxs-lookup"><span data-stu-id="24988-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24988-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="24988-112">notConfigured</span></span>|<span data-ttu-id="24988-113">0</span><span class="sxs-lookup"><span data-stu-id="24988-113">0</span></span>|<span data-ttu-id="24988-114">未指定访问级别，无意向。</span><span class="sxs-lookup"><span data-stu-id="24988-114">No access level specified, no intents.</span></span> <span data-ttu-id="24988-115">在 UserInControl 或 ForceAllow 中，设备的行为可能是一样的。</span><span class="sxs-lookup"><span data-stu-id="24988-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="24988-116">它可能取决于访问的隐私数据、Windows 版本和其他因素。</span><span class="sxs-lookup"><span data-stu-id="24988-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="24988-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="24988-117">forceAllow</span></span>|<span data-ttu-id="24988-118">1</span><span class="sxs-lookup"><span data-stu-id="24988-118">1</span></span>|<span data-ttu-id="24988-119">将允许应用访问指定的隐私数据。</span><span class="sxs-lookup"><span data-stu-id="24988-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="24988-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="24988-120">forceDeny</span></span>|<span data-ttu-id="24988-121">双面</span><span class="sxs-lookup"><span data-stu-id="24988-121">2</span></span>|<span data-ttu-id="24988-122">将拒绝应用程序访问指定的隐私数据。</span><span class="sxs-lookup"><span data-stu-id="24988-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="24988-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="24988-123">userInControl</span></span>|<span data-ttu-id="24988-124">第三章</span><span class="sxs-lookup"><span data-stu-id="24988-124">3</span></span>|<span data-ttu-id="24988-125">当应用尝试访问指定的隐私数据时，系统将提示用户。</span><span class="sxs-lookup"><span data-stu-id="24988-125">Users will be prompted when apps try to access specified privacy data.</span></span>|




