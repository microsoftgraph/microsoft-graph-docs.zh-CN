---
title: 服务根
description: 2015-10-25 14:57:30 UTC-->
localization_priority: Normal
doc_type: conceptualPageType
ms.prod: ''
author: MSGraphDocsVteam
ms.openlocfilehash: c800d75b3802d73cb0b7da4ef62d25141f9ebdee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968353"
---
# <a name="service-root"></a><span data-ttu-id="46120-103">服务根</span><span class="sxs-lookup"><span data-stu-id="46120-103">Service root</span></span>

<span data-ttu-id="46120-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46120-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a><span data-ttu-id="46120-105">方法</span><span class="sxs-lookup"><span data-stu-id="46120-105">Methods</span></span>



| <span data-ttu-id="46120-106">方法</span><span class="sxs-lookup"><span data-stu-id="46120-106">Method</span></span>           | <span data-ttu-id="46120-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="46120-107">Return Type</span></span>    |<span data-ttu-id="46120-108">说明</span><span class="sxs-lookup"><span data-stu-id="46120-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="46120-109">创建设备</span><span class="sxs-lookup"><span data-stu-id="46120-109">Create device</span></span>](../api/device-post-devices.md) |[<span data-ttu-id="46120-110">设备</span><span class="sxs-lookup"><span data-stu-id="46120-110">device</span></span>](device.md)| <span data-ttu-id="46120-111">通过发布到设备集合创建新设备。</span><span class="sxs-lookup"><span data-stu-id="46120-111">Create a new device by posting to the devices collection.</span></span>|
|[<span data-ttu-id="46120-112">列出设备</span><span class="sxs-lookup"><span data-stu-id="46120-112">List device</span></span>](../api/device-list.md) | <span data-ttu-id="46120-113">[设备](device.md)集合</span><span class="sxs-lookup"><span data-stu-id="46120-113">[device](device.md) collection</span></span> |<span data-ttu-id="46120-114">获取 device 对象集合。</span><span class="sxs-lookup"><span data-stu-id="46120-114">Get device object collection.</span></span> |
|[<span data-ttu-id="46120-115">激活 directoryRole</span><span class="sxs-lookup"><span data-stu-id="46120-115">Activate directoryRole</span></span>](../api/directoryrole-post-directoryroles.md) | [<span data-ttu-id="46120-116">directoryRole</span><span class="sxs-lookup"><span data-stu-id="46120-116">directoryRole</span></span>](directoryrole.md) |<span data-ttu-id="46120-117">激活目录角色。</span><span class="sxs-lookup"><span data-stu-id="46120-117">Activate a directory role.</span></span> |
|[<span data-ttu-id="46120-118">列出 directoryRole</span><span class="sxs-lookup"><span data-stu-id="46120-118">List directoryRole</span></span>](../api/directoryrole-list.md) | <span data-ttu-id="46120-119">[directoryRole](directoryrole.md) 集合</span><span class="sxs-lookup"><span data-stu-id="46120-119">[directoryRole](directoryrole.md) collection</span></span> |<span data-ttu-id="46120-120">获取 directoryRole 对象集合。</span><span class="sxs-lookup"><span data-stu-id="46120-120">Get directoryRole object collection.</span></span> |
|[<span data-ttu-id="46120-121">列出 directoryRoleTemplate</span><span class="sxs-lookup"><span data-stu-id="46120-121">List directoryRoleTemplate</span></span>](../api/directoryroletemplate-list.md) | <span data-ttu-id="46120-122">[directoryRoleTemplate](directoryroletemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="46120-122">[directoryRoleTemplate](directoryroletemplate.md) collection</span></span> |<span data-ttu-id="46120-123">获取 directoryRoleTemplate 对象集合。</span><span class="sxs-lookup"><span data-stu-id="46120-123">Get directoryRoleTemplate object collection.</span></span> |
|[<span data-ttu-id="46120-124">列出驱动器</span><span class="sxs-lookup"><span data-stu-id="46120-124">List drive</span></span>](../api/drive-list.md) | <span data-ttu-id="46120-125">[驱动器](drive.md) 集合</span><span class="sxs-lookup"><span data-stu-id="46120-125">[drive](drive.md) collection</span></span> |<span data-ttu-id="46120-126">获取 drive 对象集合。</span><span class="sxs-lookup"><span data-stu-id="46120-126">Get drive object collection.</span></span> |
|[<span data-ttu-id="46120-127">获取驱动器</span><span class="sxs-lookup"><span data-stu-id="46120-127">Get drive</span></span>](../api/drive-get.md) | [<span data-ttu-id="46120-128">drive</span><span class="sxs-lookup"><span data-stu-id="46120-128">drive</span></span>](drive.md)  |<span data-ttu-id="46120-129">获取 drive 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="46120-129">Get drive object properties.</span></span> |
|[<span data-ttu-id="46120-130">Create group</span><span class="sxs-lookup"><span data-stu-id="46120-130">Create group</span></span>](../api/group-post-groups.md) |[<span data-ttu-id="46120-131">组</span><span class="sxs-lookup"><span data-stu-id="46120-131">group</span></span>](group.md)| <span data-ttu-id="46120-132">通过发布到组集合创建新组。</span><span class="sxs-lookup"><span data-stu-id="46120-132">Create a new group by posting to the groups collection.</span></span>|
|[<span data-ttu-id="46120-133">列出组</span><span class="sxs-lookup"><span data-stu-id="46120-133">List group</span></span>](../api/group-list.md) | <span data-ttu-id="46120-134">[组](group.md) 集合</span><span class="sxs-lookup"><span data-stu-id="46120-134">[group](group.md) collection</span></span> |<span data-ttu-id="46120-135">获取 group 对象集合。</span><span class="sxs-lookup"><span data-stu-id="46120-135">Get group object collection.</span></span> |
|[<span data-ttu-id="46120-136">列出组织</span><span class="sxs-lookup"><span data-stu-id="46120-136">List organization</span></span>](../api/organization-list.md) | <span data-ttu-id="46120-137">[组织](organization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="46120-137">[organization](organization.md) collection</span></span> |<span data-ttu-id="46120-138">获取 organization 对象集合。</span><span class="sxs-lookup"><span data-stu-id="46120-138">Get organization object collection.</span></span> |
|[<span data-ttu-id="46120-139">列出 subscribedSku</span><span class="sxs-lookup"><span data-stu-id="46120-139">List subscribedSku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="46120-140">[subscribedSku](subscribedsku.md) 集合</span><span class="sxs-lookup"><span data-stu-id="46120-140">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="46120-141">获取 subscribedSku 对象集合。</span><span class="sxs-lookup"><span data-stu-id="46120-141">Get subscribedSku object collection.</span></span> |
|[<span data-ttu-id="46120-142">Create user</span><span class="sxs-lookup"><span data-stu-id="46120-142">Create user</span></span>](../api/user-post-users.md) |[<span data-ttu-id="46120-143">user</span><span class="sxs-lookup"><span data-stu-id="46120-143">user</span></span>](user.md)| <span data-ttu-id="46120-144">通过发布到用户集合创建新用户。</span><span class="sxs-lookup"><span data-stu-id="46120-144">Create a new user by posting to the users collection.</span></span>|
|[<span data-ttu-id="46120-145">列出用户</span><span class="sxs-lookup"><span data-stu-id="46120-145">List user</span></span>](../api/user-list.md) | <span data-ttu-id="46120-146">[用户](user.md) 集合</span><span class="sxs-lookup"><span data-stu-id="46120-146">[user](user.md) collection</span></span> |<span data-ttu-id="46120-147">获取 user 对象集合。</span><span class="sxs-lookup"><span data-stu-id="46120-147">Get user object collection.</span></span> |
|[<span data-ttu-id="46120-148">Create connectorGroup</span><span class="sxs-lookup"><span data-stu-id="46120-148">Create connectorGroup</span></span>](../api/connectorgroup-post-connectorgroups.md) |[<span data-ttu-id="46120-149">connectorGroup</span><span class="sxs-lookup"><span data-stu-id="46120-149">connectorGroup</span></span>](connectorgroup.md)|<span data-ttu-id="46120-150">通过发布到 connectorGroups 集合创建新的 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="46120-150">Create a new connectorGroup by posting to the connectorGroups collection.</span></span>|
|[<span data-ttu-id="46120-151">列出 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="46120-151">List connectorGroup</span></span>](../api/connectorgroup-list.md) | <span data-ttu-id="46120-152">[connectorGroup](connectorgroup.md) 集合</span><span class="sxs-lookup"><span data-stu-id="46120-152">[connectorGroup](connectorgroup.md) collection</span></span> |<span data-ttu-id="46120-153">获取 connectorGroup 对象集合。</span><span class="sxs-lookup"><span data-stu-id="46120-153">Get connectorGroup object collection.</span></span> |
|[<span data-ttu-id="46120-154">列表连接器</span><span class="sxs-lookup"><span data-stu-id="46120-154">List connector</span></span>](../api/connector-list.md) | <span data-ttu-id="46120-155">[连接器](connector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="46120-155">[connector](connector.md) collection</span></span> |<span data-ttu-id="46120-156">获取连接器对象集合。</span><span class="sxs-lookup"><span data-stu-id="46120-156">Get connector object collection.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


