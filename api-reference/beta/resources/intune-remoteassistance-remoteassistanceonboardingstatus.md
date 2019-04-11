---
title: remoteAssistanceOnboardingStatus 枚举类型
description: 当前 TeamViewer 连接器状态
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23490e61f4134b723cfc066043f132c44c295019
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787895"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="4ef4a-103">remoteAssistanceOnboardingStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4ef4a-103">remoteAssistanceOnboardingStatus enum type</span></span>

> <span data-ttu-id="4ef4a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4ef4a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ef4a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ef4a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ef4a-106">当前 TeamViewer 连接器状态</span><span class="sxs-lookup"><span data-stu-id="4ef4a-106">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="4ef4a-107">成员</span><span class="sxs-lookup"><span data-stu-id="4ef4a-107">Members</span></span>
|<span data-ttu-id="4ef4a-108">成员</span><span class="sxs-lookup"><span data-stu-id="4ef4a-108">Member</span></span>|<span data-ttu-id="4ef4a-109">值</span><span class="sxs-lookup"><span data-stu-id="4ef4a-109">Value</span></span>|<span data-ttu-id="4ef4a-110">说明</span><span class="sxs-lookup"><span data-stu-id="4ef4a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ef4a-111">notOnboarded</span><span class="sxs-lookup"><span data-stu-id="4ef4a-111">notOnboarded</span></span>|<span data-ttu-id="4ef4a-112">0</span><span class="sxs-lookup"><span data-stu-id="4ef4a-112">0</span></span>|<span data-ttu-id="4ef4a-113">当没有已配置或活动的活动的 TeamViewer 连接器时报告的状态</span><span class="sxs-lookup"><span data-stu-id="4ef4a-113">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="4ef4a-114">加入</span><span class="sxs-lookup"><span data-stu-id="4ef4a-114">onboarding</span></span>|<span data-ttu-id="4ef4a-115">1</span><span class="sxs-lookup"><span data-stu-id="4ef4a-115">1</span></span>|<span data-ttu-id="4ef4a-116">系统启动 TeamViewer 连接时报告的状态, 但该服务尚未完成连接器的确认</span><span class="sxs-lookup"><span data-stu-id="4ef4a-116">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="4ef4a-117">载入</span><span class="sxs-lookup"><span data-stu-id="4ef4a-117">onboarded</span></span>|<span data-ttu-id="4ef4a-118">双面</span><span class="sxs-lookup"><span data-stu-id="4ef4a-118">2</span></span>|<span data-ttu-id="4ef4a-119">系统使用 TeamViewer 成功交换帐户信息并可以立即启动与客户端的远程协助会话时报告的状态</span><span class="sxs-lookup"><span data-stu-id="4ef4a-119">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|





