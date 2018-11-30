---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
ms.openlocfilehash: 3fcfecde8dbc9efe92f842e9d2b45b7f1579c217
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046503"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="1375b-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1375b-103">appListType enum type</span></span>

> <span data-ttu-id="1375b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1375b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1375b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1375b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1375b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1375b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1375b-107">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="1375b-107">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="1375b-108">成员</span><span class="sxs-lookup"><span data-stu-id="1375b-108">Members</span></span>
|<span data-ttu-id="1375b-109">成员</span><span class="sxs-lookup"><span data-stu-id="1375b-109">Member</span></span>|<span data-ttu-id="1375b-110">值</span><span class="sxs-lookup"><span data-stu-id="1375b-110">Value</span></span>|<span data-ttu-id="1375b-111">说明</span><span class="sxs-lookup"><span data-stu-id="1375b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1375b-112">无</span><span class="sxs-lookup"><span data-stu-id="1375b-112">none</span></span>|<span data-ttu-id="1375b-113">0</span><span class="sxs-lookup"><span data-stu-id="1375b-113">0</span></span>|<span data-ttu-id="1375b-114">默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="1375b-114">Default value, no intent.</span></span>|
|<span data-ttu-id="1375b-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="1375b-115">appsInListCompliant</span></span>|<span data-ttu-id="1375b-116">1</span><span class="sxs-lookup"><span data-stu-id="1375b-116">1</span></span>|<span data-ttu-id="1375b-117">在列表代表将被视为符合 （仅在列表上的应用程序都符合） 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="1375b-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="1375b-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="1375b-118">appsNotInListCompliant</span></span>|<span data-ttu-id="1375b-119">2</span><span class="sxs-lookup"><span data-stu-id="1375b-119">2</span></span>|<span data-ttu-id="1375b-120">在列表代表将被视为不符合标准的应用程序 （所有应用程序是除列表上的应用程序兼容）。</span><span class="sxs-lookup"><span data-stu-id="1375b-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





