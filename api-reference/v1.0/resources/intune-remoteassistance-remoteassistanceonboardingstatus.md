---
title: remoteAssistanceOnboardingStatus 枚举类型
description: 当前的 TeamViewer 连接器状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8d63300e02f1442a38bbcda7f8e211e9356b8e57
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755677"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="8e4ad-103">remoteAssistanceOnboardingStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8e4ad-103">remoteAssistanceOnboardingStatus enum type</span></span>

<span data-ttu-id="8e4ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8e4ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e4ad-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e4ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e4ad-106">当前的 TeamViewer 连接器状态</span><span class="sxs-lookup"><span data-stu-id="8e4ad-106">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="8e4ad-107">成员</span><span class="sxs-lookup"><span data-stu-id="8e4ad-107">Members</span></span>
|<span data-ttu-id="8e4ad-108">成员</span><span class="sxs-lookup"><span data-stu-id="8e4ad-108">Member</span></span>|<span data-ttu-id="8e4ad-109">值</span><span class="sxs-lookup"><span data-stu-id="8e4ad-109">Value</span></span>|<span data-ttu-id="8e4ad-110">Description</span><span class="sxs-lookup"><span data-stu-id="8e4ad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e4ad-111">notOnboarded</span><span class="sxs-lookup"><span data-stu-id="8e4ad-111">notOnboarded</span></span>|<span data-ttu-id="8e4ad-112">0</span><span class="sxs-lookup"><span data-stu-id="8e4ad-112">0</span></span>|<span data-ttu-id="8e4ad-113">未配置或处于活动状态的 TeamViewer 连接器时报告的状态</span><span class="sxs-lookup"><span data-stu-id="8e4ad-113">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="8e4ad-114">载入</span><span class="sxs-lookup"><span data-stu-id="8e4ad-114">onboarding</span></span>|<span data-ttu-id="8e4ad-115">1</span><span class="sxs-lookup"><span data-stu-id="8e4ad-115">1</span></span>|<span data-ttu-id="8e4ad-116">当系统启动 TeamViewer 连接，但服务尚未完成连接器确认时报告的状态</span><span class="sxs-lookup"><span data-stu-id="8e4ad-116">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="8e4ad-117">已载入</span><span class="sxs-lookup"><span data-stu-id="8e4ad-117">onboarded</span></span>|<span data-ttu-id="8e4ad-118">2</span><span class="sxs-lookup"><span data-stu-id="8e4ad-118">2</span></span>|<span data-ttu-id="8e4ad-119">当系统已成功与 TeamViewer 交换帐户信息，并且现在可以与客户端启动远程协助会话时报告的状态</span><span class="sxs-lookup"><span data-stu-id="8e4ad-119">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|




