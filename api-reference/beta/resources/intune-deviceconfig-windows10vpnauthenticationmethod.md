---
title: windows10VpnAuthenticationMethod 枚举类型
description: Windows 10 VPN 连接类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aa011b6231f6b430fcefcc36affbf92c2fd5d717
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418489"
---
# <a name="windows10vpnauthenticationmethod-enum-type"></a><span data-ttu-id="83c7a-103">windows10VpnAuthenticationMethod 枚举类型</span><span class="sxs-lookup"><span data-stu-id="83c7a-103">windows10VpnAuthenticationMethod enum type</span></span>

> <span data-ttu-id="83c7a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="83c7a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="83c7a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="83c7a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83c7a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83c7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83c7a-107">Windows 10 VPN 连接类型。</span><span class="sxs-lookup"><span data-stu-id="83c7a-107">Windows 10 VPN connection types.</span></span>

## <a name="members"></a><span data-ttu-id="83c7a-108">成员</span><span class="sxs-lookup"><span data-stu-id="83c7a-108">Members</span></span>
|<span data-ttu-id="83c7a-109">成员</span><span class="sxs-lookup"><span data-stu-id="83c7a-109">Member</span></span>|<span data-ttu-id="83c7a-110">值</span><span class="sxs-lookup"><span data-stu-id="83c7a-110">Value</span></span>|<span data-ttu-id="83c7a-111">说明</span><span class="sxs-lookup"><span data-stu-id="83c7a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83c7a-112">certificate</span><span class="sxs-lookup"><span data-stu-id="83c7a-112">certificate</span></span>|<span data-ttu-id="83c7a-113">0</span><span class="sxs-lookup"><span data-stu-id="83c7a-113">0</span></span>|<span data-ttu-id="83c7a-114">使用证书进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="83c7a-114">Authenticate with a certificate.</span></span>|
|<span data-ttu-id="83c7a-115">usernameAndPassword</span><span class="sxs-lookup"><span data-stu-id="83c7a-115">usernameAndPassword</span></span>|<span data-ttu-id="83c7a-116">1</span><span class="sxs-lookup"><span data-stu-id="83c7a-116">1</span></span>|<span data-ttu-id="83c7a-117">用于身份验证的用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="83c7a-117">Use username and password for authentication.</span></span>|
|<span data-ttu-id="83c7a-118">customEapXml</span><span class="sxs-lookup"><span data-stu-id="83c7a-118">customEapXml</span></span>|<span data-ttu-id="83c7a-119">2</span><span class="sxs-lookup"><span data-stu-id="83c7a-119">2</span></span>|<span data-ttu-id="83c7a-120">自定义 EAP XML 中指定身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="83c7a-120">Authentication method is specified in custom EAP XML.</span></span>|




