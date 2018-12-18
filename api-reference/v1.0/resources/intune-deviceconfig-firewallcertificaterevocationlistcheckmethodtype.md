---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
author: tfitzmac
ms.openlocfilehash: ab496b5deb8f096bdc48a2b50a1af994c8ec8d5b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353660"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="a86e8-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a86e8-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="a86e8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a86e8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a86e8-105">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="a86e8-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="a86e8-106">成员</span><span class="sxs-lookup"><span data-stu-id="a86e8-106">Members</span></span>
|<span data-ttu-id="a86e8-107">成员</span><span class="sxs-lookup"><span data-stu-id="a86e8-107">Member</span></span>|<span data-ttu-id="a86e8-108">值</span><span class="sxs-lookup"><span data-stu-id="a86e8-108">Value</span></span>|<span data-ttu-id="a86e8-109">说明</span><span class="sxs-lookup"><span data-stu-id="a86e8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a86e8-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="a86e8-110">deviceDefault</span></span>|<span data-ttu-id="a86e8-111">0</span><span class="sxs-lookup"><span data-stu-id="a86e8-111">0</span></span>|<span data-ttu-id="a86e8-112">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="a86e8-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="a86e8-113">无</span><span class="sxs-lookup"><span data-stu-id="a86e8-113">none</span></span>|<span data-ttu-id="a86e8-114">1</span><span class="sxs-lookup"><span data-stu-id="a86e8-114">1</span></span>|<span data-ttu-id="a86e8-115">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="a86e8-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="a86e8-116">尝试</span><span class="sxs-lookup"><span data-stu-id="a86e8-116">attempt</span></span>|<span data-ttu-id="a86e8-117">2</span><span class="sxs-lookup"><span data-stu-id="a86e8-117">2</span></span>|<span data-ttu-id="a86e8-118">尝试 CRL 检查并检查确认证书时才允许证书</span><span class="sxs-lookup"><span data-stu-id="a86e8-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="a86e8-119">需要</span><span class="sxs-lookup"><span data-stu-id="a86e8-119">require</span></span>|<span data-ttu-id="a86e8-120">3</span><span class="sxs-lookup"><span data-stu-id="a86e8-120">3</span></span>|<span data-ttu-id="a86e8-121">需要之前允许证书的 CRL 检查成功</span><span class="sxs-lookup"><span data-stu-id="a86e8-121">Require a successful CRL check before allowing a certificate</span></span>|



