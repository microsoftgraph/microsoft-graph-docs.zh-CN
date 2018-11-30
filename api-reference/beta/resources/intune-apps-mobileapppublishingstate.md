---
title: mobileAppPublishingState 枚举类型
description: 指示应用程序的发布状态。
ms.openlocfilehash: bea64eb6d882660c91b938c95004da3ad67792a7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047477"
---
# <a name="mobileapppublishingstate-enum-type"></a><span data-ttu-id="ab4ff-103">mobileAppPublishingState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ab4ff-103">mobileAppPublishingState enum type</span></span>

> <span data-ttu-id="ab4ff-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ab4ff-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab4ff-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ab4ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab4ff-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ab4ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab4ff-107">指示应用程序的发布状态。</span><span class="sxs-lookup"><span data-stu-id="ab4ff-107">Indicates the publishing state of an app.</span></span>
## <a name="members"></a><span data-ttu-id="ab4ff-108">成员</span><span class="sxs-lookup"><span data-stu-id="ab4ff-108">Members</span></span>
|<span data-ttu-id="ab4ff-109">成员</span><span class="sxs-lookup"><span data-stu-id="ab4ff-109">Member</span></span>|<span data-ttu-id="ab4ff-110">值</span><span class="sxs-lookup"><span data-stu-id="ab4ff-110">Value</span></span>|<span data-ttu-id="ab4ff-111">说明</span><span class="sxs-lookup"><span data-stu-id="ab4ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab4ff-112">notPublished</span><span class="sxs-lookup"><span data-stu-id="ab4ff-112">notPublished</span></span>|<span data-ttu-id="ab4ff-113">0</span><span class="sxs-lookup"><span data-stu-id="ab4ff-113">0</span></span>|<span data-ttu-id="ab4ff-114">尚未发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="ab4ff-114">The app is not yet published.</span></span>|
|<span data-ttu-id="ab4ff-115">处理</span><span class="sxs-lookup"><span data-stu-id="ab4ff-115">processing</span></span>|<span data-ttu-id="ab4ff-116">1</span><span class="sxs-lookup"><span data-stu-id="ab4ff-116">1</span></span>|<span data-ttu-id="ab4ff-117">待处理的服务商处理应用程序。</span><span class="sxs-lookup"><span data-stu-id="ab4ff-117">The app is pending service-side processing.</span></span>|
|<span data-ttu-id="ab4ff-118">已发布</span><span class="sxs-lookup"><span data-stu-id="ab4ff-118">published</span></span>|<span data-ttu-id="ab4ff-119">2</span><span class="sxs-lookup"><span data-stu-id="ab4ff-119">2</span></span>|<span data-ttu-id="ab4ff-120">发布应用程序。</span><span class="sxs-lookup"><span data-stu-id="ab4ff-120">The app is published.</span></span>|





