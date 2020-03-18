---
title: remoteAssistanceOnboardingStatus 枚举类型
description: 当前 TeamViewer 连接器状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 68e5a8bff7f1753540a2716a00fd9148e188d7ea
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42772935"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a><span data-ttu-id="d31fc-103">remoteAssistanceOnboardingStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d31fc-103">remoteAssistanceOnboardingStatus enum type</span></span>

> <span data-ttu-id="d31fc-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d31fc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d31fc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d31fc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d31fc-106">当前 TeamViewer 连接器状态</span><span class="sxs-lookup"><span data-stu-id="d31fc-106">The current TeamViewer connector status</span></span>

## <a name="members"></a><span data-ttu-id="d31fc-107">成员</span><span class="sxs-lookup"><span data-stu-id="d31fc-107">Members</span></span>
|<span data-ttu-id="d31fc-108">成员</span><span class="sxs-lookup"><span data-stu-id="d31fc-108">Member</span></span>|<span data-ttu-id="d31fc-109">值</span><span class="sxs-lookup"><span data-stu-id="d31fc-109">Value</span></span>|<span data-ttu-id="d31fc-110">说明</span><span class="sxs-lookup"><span data-stu-id="d31fc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d31fc-111">notOnboarded</span><span class="sxs-lookup"><span data-stu-id="d31fc-111">notOnboarded</span></span>|<span data-ttu-id="d31fc-112">0</span><span class="sxs-lookup"><span data-stu-id="d31fc-112">0</span></span>|<span data-ttu-id="d31fc-113">当没有已配置或活动的活动的 TeamViewer 连接器时报告的状态</span><span class="sxs-lookup"><span data-stu-id="d31fc-113">The status reported when there is no active TeamViewer connector configured or active</span></span>|
|<span data-ttu-id="d31fc-114">加入</span><span class="sxs-lookup"><span data-stu-id="d31fc-114">onboarding</span></span>|<span data-ttu-id="d31fc-115">1</span><span class="sxs-lookup"><span data-stu-id="d31fc-115">1</span></span>|<span data-ttu-id="d31fc-116">系统启动 TeamViewer 连接时报告的状态，但该服务尚未完成连接器的确认</span><span class="sxs-lookup"><span data-stu-id="d31fc-116">The status reported when the system has initiated a TeamViewer connection, but the service has not yet completed the confirmation of a connector</span></span>|
|<span data-ttu-id="d31fc-117">载入</span><span class="sxs-lookup"><span data-stu-id="d31fc-117">onboarded</span></span>|<span data-ttu-id="d31fc-118">双面</span><span class="sxs-lookup"><span data-stu-id="d31fc-118">2</span></span>|<span data-ttu-id="d31fc-119">系统使用 TeamViewer 成功交换帐户信息并可以立即启动与客户端的远程协助会话时报告的状态</span><span class="sxs-lookup"><span data-stu-id="d31fc-119">The status reported when the system has successfully exchanged account information with TeamViewer and can now initiate remote assistance sessions with clients</span></span>|



