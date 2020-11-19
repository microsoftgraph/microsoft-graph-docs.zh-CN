---
title: iosNotificationPreviewVisibility 枚举类型
description: 确定何时在 iOS 设备上显示通知预览。 预览可以包括文本 (来自) 日历) 中的邮件和邮件和邀请详细 (信息等内容。 配置后，它将覆盖用户定义的预览设置。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 607e771ce83858cd22892efa9a377b7997142a24
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301601"
---
# <a name="iosnotificationpreviewvisibility-enum-type"></a><span data-ttu-id="ea91f-105">iosNotificationPreviewVisibility 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ea91f-105">iosNotificationPreviewVisibility enum type</span></span>

<span data-ttu-id="ea91f-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea91f-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea91f-107">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea91f-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea91f-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea91f-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea91f-109">确定何时在 iOS 设备上显示通知预览。</span><span class="sxs-lookup"><span data-stu-id="ea91f-109">Determines when notification previews are visible on an iOS device.</span></span> <span data-ttu-id="ea91f-110">预览可以包括文本 (来自) 日历) 中的邮件和邮件和邀请详细 (信息等内容。</span><span class="sxs-lookup"><span data-stu-id="ea91f-110">Previews can include things like text (from Messages and Mail) and invitation details (from Calendar).</span></span> <span data-ttu-id="ea91f-111">配置后，它将覆盖用户定义的预览设置。</span><span class="sxs-lookup"><span data-stu-id="ea91f-111">When configured, it will override the user's defined preview settings.</span></span>

## <a name="members"></a><span data-ttu-id="ea91f-112">成员</span><span class="sxs-lookup"><span data-stu-id="ea91f-112">Members</span></span>
|<span data-ttu-id="ea91f-113">成员</span><span class="sxs-lookup"><span data-stu-id="ea91f-113">Member</span></span>|<span data-ttu-id="ea91f-114">值</span><span class="sxs-lookup"><span data-stu-id="ea91f-114">Value</span></span>|<span data-ttu-id="ea91f-115">Description</span><span class="sxs-lookup"><span data-stu-id="ea91f-115">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea91f-116">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ea91f-116">notConfigured</span></span>|<span data-ttu-id="ea91f-117">0</span><span class="sxs-lookup"><span data-stu-id="ea91f-117">0</span></span>|<span data-ttu-id="ea91f-118">通知预览设置不会被覆盖。</span><span class="sxs-lookup"><span data-stu-id="ea91f-118">Notification preview settings will not be overwritten.</span></span>|
|<span data-ttu-id="ea91f-119">alwaysShow</span><span class="sxs-lookup"><span data-stu-id="ea91f-119">alwaysShow</span></span>|<span data-ttu-id="ea91f-120">1</span><span class="sxs-lookup"><span data-stu-id="ea91f-120">1</span></span>|<span data-ttu-id="ea91f-121">始终显示通知预览。</span><span class="sxs-lookup"><span data-stu-id="ea91f-121">Always show notification previews.</span></span>|
|<span data-ttu-id="ea91f-122">hideWhenLocked</span><span class="sxs-lookup"><span data-stu-id="ea91f-122">hideWhenLocked</span></span>|<span data-ttu-id="ea91f-123">双面</span><span class="sxs-lookup"><span data-stu-id="ea91f-123">2</span></span>|<span data-ttu-id="ea91f-124">设备处于解锁状态时仅显示通知预览。</span><span class="sxs-lookup"><span data-stu-id="ea91f-124">Only show notification previews when the device is unlocked.</span></span>|
|<span data-ttu-id="ea91f-125">neverShow</span><span class="sxs-lookup"><span data-stu-id="ea91f-125">neverShow</span></span>|<span data-ttu-id="ea91f-126">第三章</span><span class="sxs-lookup"><span data-stu-id="ea91f-126">3</span></span>|<span data-ttu-id="ea91f-127">从不显示通知预览。</span><span class="sxs-lookup"><span data-stu-id="ea91f-127">Never show notification previews.</span></span>|




