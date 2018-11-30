---
title: firewallCertificateRevocationListCheckMethodType 枚举类型
description: FirewallCertificateRevocationListCheckMethod 的可能值
ms.openlocfilehash: b6a7d702b1156598387c204d9e42b15f3066598d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010370"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="9315c-103">firewallCertificateRevocationListCheckMethodType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9315c-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="9315c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9315c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9315c-105">FirewallCertificateRevocationListCheckMethod 的可能值</span><span class="sxs-lookup"><span data-stu-id="9315c-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="9315c-106">成员</span><span class="sxs-lookup"><span data-stu-id="9315c-106">Members</span></span>
|<span data-ttu-id="9315c-107">成员</span><span class="sxs-lookup"><span data-stu-id="9315c-107">Member</span></span>|<span data-ttu-id="9315c-108">值</span><span class="sxs-lookup"><span data-stu-id="9315c-108">Value</span></span>|<span data-ttu-id="9315c-109">说明</span><span class="sxs-lookup"><span data-stu-id="9315c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9315c-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="9315c-110">deviceDefault</span></span>|<span data-ttu-id="9315c-111">0</span><span class="sxs-lookup"><span data-stu-id="9315c-111">0</span></span>|<span data-ttu-id="9315c-112">配置通过 Intune，没有值不会替代的用户配置设备默认值</span><span class="sxs-lookup"><span data-stu-id="9315c-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="9315c-113">无</span><span class="sxs-lookup"><span data-stu-id="9315c-113">none</span></span>|<span data-ttu-id="9315c-114">1</span><span class="sxs-lookup"><span data-stu-id="9315c-114">1</span></span>|<span data-ttu-id="9315c-115">不检查证书吊销列表</span><span class="sxs-lookup"><span data-stu-id="9315c-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="9315c-116">尝试</span><span class="sxs-lookup"><span data-stu-id="9315c-116">attempt</span></span>|<span data-ttu-id="9315c-117">2</span><span class="sxs-lookup"><span data-stu-id="9315c-117">2</span></span>|<span data-ttu-id="9315c-118">尝试 CRL 检查并检查确认证书时才允许证书</span><span class="sxs-lookup"><span data-stu-id="9315c-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="9315c-119">需要</span><span class="sxs-lookup"><span data-stu-id="9315c-119">require</span></span>|<span data-ttu-id="9315c-120">3</span><span class="sxs-lookup"><span data-stu-id="9315c-120">3</span></span>|<span data-ttu-id="9315c-121">需要之前允许证书的 CRL 检查成功</span><span class="sxs-lookup"><span data-stu-id="9315c-121">Require a successful CRL check before allowing a certificate</span></span>|



