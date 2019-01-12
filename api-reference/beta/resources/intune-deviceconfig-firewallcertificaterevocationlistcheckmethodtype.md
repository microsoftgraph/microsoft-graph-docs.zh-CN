---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 915fab77e7a2c28ab9d6902f3e1cb7d2d05cb2b0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958409"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="81b81-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="81b81-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="81b81-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="81b81-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81b81-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="81b81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81b81-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="81b81-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81b81-107">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="81b81-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="81b81-108">成员</span><span class="sxs-lookup"><span data-stu-id="81b81-108">Members</span></span>
|<span data-ttu-id="81b81-109">成员</span><span class="sxs-lookup"><span data-stu-id="81b81-109">Member</span></span>|<span data-ttu-id="81b81-110">值</span><span class="sxs-lookup"><span data-stu-id="81b81-110">Value</span></span>|<span data-ttu-id="81b81-111">Description</span><span class="sxs-lookup"><span data-stu-id="81b81-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81b81-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="81b81-112">deviceDefault</span></span>|<span data-ttu-id="81b81-113">0</span><span class="sxs-lookup"><span data-stu-id="81b81-113">0</span></span>|<span data-ttu-id="81b81-114">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="81b81-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="81b81-115">无</span><span class="sxs-lookup"><span data-stu-id="81b81-115">none</span></span>|<span data-ttu-id="81b81-116">1</span><span class="sxs-lookup"><span data-stu-id="81b81-116">1</span></span>|<span data-ttu-id="81b81-117">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="81b81-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="81b81-118">尝试</span><span class="sxs-lookup"><span data-stu-id="81b81-118">attempt</span></span>|<span data-ttu-id="81b81-119">2</span><span class="sxs-lookup"><span data-stu-id="81b81-119">2</span></span>|<span data-ttu-id="81b81-120">尝试 CRL 检查并检查确认证书时才允许证书</span><span class="sxs-lookup"><span data-stu-id="81b81-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="81b81-121">需要</span><span class="sxs-lookup"><span data-stu-id="81b81-121">require</span></span>|<span data-ttu-id="81b81-122">3</span><span class="sxs-lookup"><span data-stu-id="81b81-122">3</span></span>|<span data-ttu-id="81b81-123">需要之前允许证书的 CRL 检查成功</span><span class="sxs-lookup"><span data-stu-id="81b81-123">Require a successful CRL check before allowing a certificate</span></span>|





