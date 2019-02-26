---
title: 在 Intune 中管理资源访问证书-Microsoft Graph API
description: 列出管理租户组织的资源访问证书的适用于 Intune 终结点 (REST) 的 Microsoft Graph API。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 943597fc6d1b133ec29e87d544c016f6c2ab703f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168136"
---
# <a name="manage-resource-access-certificates-in-intune"></a><span data-ttu-id="4f77a-103">在 Intune 中管理资源访问证书</span><span class="sxs-lookup"><span data-stu-id="4f77a-103">Manage resource access certificates in Intune</span></span>

> <span data-ttu-id="4f77a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4f77a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4f77a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4f77a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4f77a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4f77a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="4f77a-107">您可以使用 Microsoft Graph API 为 Intune 导入 PFX 证书。</span><span class="sxs-lookup"><span data-stu-id="4f77a-107">You can import PFX certificates using Microsoft Graph API for Intune.</span></span>

<span data-ttu-id="4f77a-108">以下 Graph 资源可用于在 Intune 中管理注册：</span><span class="sxs-lookup"><span data-stu-id="4f77a-108">The following Graph resources are available to manage enrollment in Intune:</span></span>

- [<span data-ttu-id="4f77a-109">用户 PFX 证书</span><span class="sxs-lookup"><span data-stu-id="4f77a-109">User PFX certificate</span></span>](intune-raimportcerts-userpfxcertificate.md)
- [<span data-ttu-id="4f77a-110">用户 PFX 预期目的</span><span class="sxs-lookup"><span data-stu-id="4f77a-110">User PFX intended purpose</span></span>](intune-raimportcerts-userpfxintendedpurpose.md)
- [<span data-ttu-id="4f77a-111">用户 PFX 填充方案</span><span class="sxs-lookup"><span data-stu-id="4f77a-111">User PFX padding scheme</span></span>](intune-raimportcerts-userpfxpaddingscheme.md)
