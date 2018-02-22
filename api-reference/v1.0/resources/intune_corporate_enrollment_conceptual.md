# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="d4404-101">使用 Intune 注册企业拥有的设备</span><span class="sxs-lookup"><span data-stu-id="d4404-101">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="d4404-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://www.microsoft.com/zh-CN/cloud-platform/microsoft-intune-pricing) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d4404-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/zh-CN/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="d4404-103">通过 Intune，你可以用多种方式注册要管理的组织拥有或企业拥有的设备，具体取决于设备的类型、设备的购买方式和组织的需求。</span><span class="sxs-lookup"><span data-stu-id="d4404-103">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="d4404-104">你还可以安装公司门户应用，注册和管理企业拥有的设备，例如，在“自带设备”(BYOD) 场景中进行管理。</span><span class="sxs-lookup"><span data-stu-id="d4404-104">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="d4404-105">以下 Graph 资源可用于在 Intune 中管理企业拥有的设备：</span><span class="sxs-lookup"><span data-stu-id="d4404-105">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="d4404-106">所有设备分配目标</span><span class="sxs-lookup"><span data-stu-id="d4404-106">All devices assignment target</span></span>](intune_onboarding_alldevicesassignmenttarget.md)
- [<span data-ttu-id="d4404-107">所有许可的用户分配目标</span><span class="sxs-lookup"><span data-stu-id="d4404-107">All licensed users assignment target</span></span>](intune_onboarding_alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="d4404-108">设备和应用管理分配目标</span><span class="sxs-lookup"><span data-stu-id="d4404-108">Device and app management assignment target</span></span>](intune_onboarding_deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="d4404-109">设备应用管理</span><span class="sxs-lookup"><span data-stu-id="d4404-109">Device app management</span></span>](intune_onboarding_deviceappmanagement.md)
- [<span data-ttu-id="d4404-110">设备类别</span><span class="sxs-lookup"><span data-stu-id="d4404-110">Device category</span></span>](intune_onboarding_devicecategory.md)
- [<span data-ttu-id="d4404-111">设备注册配置</span><span class="sxs-lookup"><span data-stu-id="d4404-111">Device enrollment configuration</span></span>](intune_onboarding_deviceenrollmentconfiguration.md)
- [<span data-ttu-id="d4404-112">设备注册限制配置</span><span class="sxs-lookup"><span data-stu-id="d4404-112">Device enrollment limit configuration</span></span>](intune_onboarding_deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="d4404-113">设备注册平台限制</span><span class="sxs-lookup"><span data-stu-id="d4404-113">Device enrollment platform restriction</span></span>](intune_onboarding_deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="d4404-114">设备注册平台限制配置</span><span class="sxs-lookup"><span data-stu-id="d4404-114">Device enrollment platform restrictions configuration</span></span>](intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="d4404-115">设备注册 Windows Hello 企业版配置</span><span class="sxs-lookup"><span data-stu-id="d4404-115">Device enrollment Windows Hello for business configuration</span></span>](intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="d4404-116">设备管理 Exchange 连接器</span><span class="sxs-lookup"><span data-stu-id="d4404-116">Device management exchange connector</span></span>](intune_onboarding_devicemanagementexchangeconnector.md)
- [<span data-ttu-id="d4404-117">设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="d4404-117">Device management partner</span></span>](intune_onboarding_devicemanagementpartner.md)
- [<span data-ttu-id="d4404-118">设备管理</span><span class="sxs-lookup"><span data-stu-id="d4404-118">Device management</span></span>](intune_onboarding_devicemanagement.md)
- [<span data-ttu-id="d4404-119">注册配置分配</span><span class="sxs-lookup"><span data-stu-id="d4404-119">Enrollment configuration assignment</span></span>](intune_onboarding_enrollmentconfigurationassignment.md)
- [<span data-ttu-id="d4404-120">排除组分配目标</span><span class="sxs-lookup"><span data-stu-id="d4404-120">Exclusion group assignment target</span></span>](intune_onboarding_exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="d4404-121">组分配目标</span><span class="sxs-lookup"><span data-stu-id="d4404-121">Group assignment target</span></span>](intune_onboarding_groupassignmenttarget.md)
- [<span data-ttu-id="d4404-122">Intune 品牌</span><span class="sxs-lookup"><span data-stu-id="d4404-122">Intune brand</span></span>](intune_onboarding_intunebrand.md)
- [<span data-ttu-id="d4404-123">MIME 内容</span><span class="sxs-lookup"><span data-stu-id="d4404-123">MIME content</span></span>](intune_onboarding_mimecontent.md)
- [<span data-ttu-id="d4404-124">移动威胁防护连接器</span><span class="sxs-lookup"><span data-stu-id="d4404-124">Mobile threat defense connector</span></span>](intune_onboarding_mobilethreatdefenseconnector.md)
- [<span data-ttu-id="d4404-125">本地条件访问设置</span><span class="sxs-lookup"><span data-stu-id="d4404-125">On-premises conditional access settings</span></span>](intune_onboarding_onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="d4404-126">组织</span><span class="sxs-lookup"><span data-stu-id="d4404-126">Organization</span></span>](intune_onboarding_organization.md)
- [<span data-ttu-id="d4404-127">RGB 颜色</span><span class="sxs-lookup"><span data-stu-id="d4404-127">RGB color</span></span>](intune_onboarding_rgbcolor.md)
- [<span data-ttu-id="d4404-128">用户</span><span class="sxs-lookup"><span data-stu-id="d4404-128">User</span></span>](intune_onboarding_user.md)
