---
title: remoteAssistanceOnboardingStatus 枚举类型
description: 当前 TeamViewer 连接器状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ccb04964c7608c24ec8822bac7832aaf77bdfd7f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287786"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="c4928-103">remoteAssistanceOnboardingStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c4928-103">remoteAssistanceOnboardingStatus enum type</span></span>

<span data-ttu-id="c4928-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4928-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4928-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c4928-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4928-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c4928-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4928-107">当前 TeamViewer 连接器状态</span><span class="sxs-lookup"><span data-stu-id="c4928-107">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="c4928-108">成员</span><span class="sxs-lookup"><span data-stu-id="c4928-108">Members</span></span>
|<span data-ttu-id="c4928-109">成员</span><span class="sxs-lookup"><span data-stu-id="c4928-109">Member</span></span>|<span data-ttu-id="c4928-110">值</span><span class="sxs-lookup"><span data-stu-id="c4928-110">Value</span></span>|<span data-ttu-id="c4928-111">Description</span><span class="sxs-lookup"><span data-stu-id="c4928-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4928-112">notOnboarded</span><span class="sxs-lookup"><span data-stu-id="c4928-112">notOnboarded</span></span>|<span data-ttu-id="c4928-113">0</span><span class="sxs-lookup"><span data-stu-id="c4928-113">0</span></span>|<span data-ttu-id="c4928-114">当没有已配置或活动的活动的 TeamViewer 连接器时报告的状态</span><span class="sxs-lookup"><span data-stu-id="c4928-114">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="c4928-115">加入</span><span class="sxs-lookup"><span data-stu-id="c4928-115">onboarding</span></span>|<span data-ttu-id="c4928-116">1</span><span class="sxs-lookup"><span data-stu-id="c4928-116">1</span></span>|<span data-ttu-id="c4928-117">系统启动 TeamViewer 连接时报告的状态，但该服务尚未完成连接器的确认</span><span class="sxs-lookup"><span data-stu-id="c4928-117">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="c4928-118">载入</span><span class="sxs-lookup"><span data-stu-id="c4928-118">onboarded</span></span>|<span data-ttu-id="c4928-119">双面</span><span class="sxs-lookup"><span data-stu-id="c4928-119">2</span></span>|<span data-ttu-id="c4928-120">系统使用 TeamViewer 成功交换帐户信息并可以立即启动与客户端的远程协助会话时报告的状态</span><span class="sxs-lookup"><span data-stu-id="c4928-120">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|




