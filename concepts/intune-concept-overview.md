# <a name="intune-devices-and-apps-api-overview"></a><span data-ttu-id="ea93a-101">Intune 设备和应用 API 概述</span><span class="sxs-lookup"><span data-stu-id="ea93a-101">Intune devices and apps API overview</span></span>

<span data-ttu-id="ea93a-102">Microsoft Intune 可帮助企业管理组织内的设备和应用。</span><span class="sxs-lookup"><span data-stu-id="ea93a-102">Microsoft Intune helps enterprises manage devices and apps within an organization.</span></span> <span data-ttu-id="ea93a-103">你可以使用 Microsoft Graph 中的 Intune API 来管理设备和应用，甚至可以在使用首选工具时配置 Intune。</span><span class="sxs-lookup"><span data-stu-id="ea93a-103">You can use the Intune API in Microsoft Graph to manage devices, apps, and even configure Intune while using your preferred tools.</span></span> 

<span data-ttu-id="ea93a-104">如果你是 ISV，则还可以使用 Intune API 来管理客户端租户。</span><span class="sxs-lookup"><span data-stu-id="ea93a-104">If you're an ISV, you can also use the Intune API to manage client tenants.</span></span>

## <a name="why-integrate-with-intune"></a><span data-ttu-id="ea93a-105">为什么与 Intune 集成？</span><span class="sxs-lookup"><span data-stu-id="ea93a-105">Why integrate with Intune?</span></span>

<span data-ttu-id="ea93a-106">你可以使用 Microsoft Graph 中的 Intune API 访问 Intune 设备和应用程序信息，管理设备、管理应用和自动执行 Intune。</span><span class="sxs-lookup"><span data-stu-id="ea93a-106">You can use the Intune API in Microsoft Graph to access Intune device and application information, manage devices, manage apps, and automate Intune.</span></span>

### <a name="manage-devices"></a><span data-ttu-id="ea93a-107">管理设备</span><span class="sxs-lookup"><span data-stu-id="ea93a-107">Manage devices</span></span>

<span data-ttu-id="ea93a-108">可以使用 Intune API 执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="ea93a-108">You can use the Intune API to:</span></span>

- <span data-ttu-id="ea93a-109">定义并强制实施[设备合规性](../api-reference/v1.0/resources/intune_deviceconfig_devicecomplianceactionitem.md)策略，例如密码复杂性和持续时间、加密、威胁保护级别等。</span><span class="sxs-lookup"><span data-stu-id="ea93a-109">Define and enforce [device compliance](../api-reference/v1.0/resources/intune_deviceconfig_devicecomplianceactionitem.md) policies, such as password complexity and duration, encryption, threat protection levels, and so on.</span></span>  <span data-ttu-id="ea93a-110">（支持的策略会根据操作系统和版本的不同而异）。</span><span class="sxs-lookup"><span data-stu-id="ea93a-110">(Supported policies vary according to operating system and version).</span></span>
- <span data-ttu-id="ea93a-111">[保护公司数据](../api-reference/v1.0/resources/intune_mam_windowsinformationprotectionpolicy.md)，无论设备平台是 Windows、Android、Mac 还是 iOS。</span><span class="sxs-lookup"><span data-stu-id="ea93a-111">[Protect company data](../api-reference/v1.0/resources/intune_mam_windowsinformationprotectionpolicy.md), regardless of whether the device platform is Windows, Android, Mac, or iOS.</span></span>
- <span data-ttu-id="ea93a-112">创建和部署[设备配置](../api-reference/v1.0/resources/intune_deviceconfig_deviceconfiguration.md)策略，包括操作系统平台/版本控制、域成员身份和配置设置管理。</span><span class="sxs-lookup"><span data-stu-id="ea93a-112">Create and deploy [device configuration](../api-reference/v1.0/resources/intune_deviceconfig_deviceconfiguration.md) policies, including operating system platform/versioning, domain membership, and configuration setting management.</span></span>
- <span data-ttu-id="ea93a-113">创建和部署设备[访问控制](../api-reference/v1.0/resources/intune_onboarding_onpremisesconditionalaccesssettings.md)策略，包括受限的下载、网络附件访问和文件传输。</span><span class="sxs-lookup"><span data-stu-id="ea93a-113">Create and deploy device [access control](../api-reference/v1.0/resources/intune_onboarding_onpremisesconditionalaccesssettings.md) policies, including restricted download, network accessory access, and file transfer.</span></span>
- <span data-ttu-id="ea93a-114">执行[远程操作](../api-reference/v1.0/resources/intune_devices_manageddevice.md)，如定位设备、更改密码和擦除设备。</span><span class="sxs-lookup"><span data-stu-id="ea93a-114">Perform [remote actions](../api-reference/v1.0/resources/intune_devices_manageddevice.md), such as locate device, change password, and wipe device.</span></span>

### <a name="manage-apps"></a><span data-ttu-id="ea93a-115">管理应用</span><span class="sxs-lookup"><span data-stu-id="ea93a-115">Manage apps</span></span> 

<span data-ttu-id="ea93a-116">Intune API 可用于执行下列应用管理任务：</span><span class="sxs-lookup"><span data-stu-id="ea93a-116">You can use the Intune API to perform the following app management tasks:</span></span>

- <span data-ttu-id="ea93a-117">[将应用部署到设备](../api-reference/v1.0/resources/intune_apps_mobileapp.md)或阻止部署应用。</span><span class="sxs-lookup"><span data-stu-id="ea93a-117">Deploy [apps to devices](../api-reference/v1.0/resources/intune_apps_mobileapp.md) or prevent apps from being deployed.</span></span>
- <span data-ttu-id="ea93a-118">管理对[电子书](../api-reference/v1.0/resources/intune_books_ebookinstallsummary.md)及相关服务的访问。</span><span class="sxs-lookup"><span data-stu-id="ea93a-118">Manage access to [ebooks](../api-reference/v1.0/resources/intune_books_ebookinstallsummary.md) and related services.</span></span>
- <span data-ttu-id="ea93a-119">定义和部署应用配置设置、应用保护设置和应用使用策略。</span><span class="sxs-lookup"><span data-stu-id="ea93a-119">Define and deploy app configuration settings, app protection settings, and app usage policies.</span></span>

### <a name="automate-intune"></a><span data-ttu-id="ea93a-120">自动执行 Intune</span><span class="sxs-lookup"><span data-stu-id="ea93a-120">Automate Intune</span></span>

<span data-ttu-id="ea93a-121">使用 Intune API 自动执行 Intune 可进行以下操作：</span><span class="sxs-lookup"><span data-stu-id="ea93a-121">Automate Intune by using the Intune API to:</span></span>

- <span data-ttu-id="ea93a-122">定义和分配[基于角色的](../api-reference/v1.0/resources/intune_rbac_conceptual.md)访问控件。</span><span class="sxs-lookup"><span data-stu-id="ea93a-122">Define and assign [role based](../api-reference/v1.0/resources/intune_rbac_conceptual.md) access controls.</span></span>
- <span data-ttu-id="ea93a-123">审核和报告合规性、使用情况和访问权限。</span><span class="sxs-lookup"><span data-stu-id="ea93a-123">Audit and report compliance, usage, and access.</span></span>
- <span data-ttu-id="ea93a-124">管理[电信费用](../api-reference/v1.0/resources/intune_tem_conceptual.md)。</span><span class="sxs-lookup"><span data-stu-id="ea93a-124">Manage [telecom expenses](../api-reference/v1.0/resources/intune_tem_conceptual.md).</span></span>


## <a name="next-steps"></a><span data-ttu-id="ea93a-125">后续步骤</span><span class="sxs-lookup"><span data-stu-id="ea93a-125">Next steps</span></span>

- <span data-ttu-id="ea93a-126">[使用 Azure AD 访问 Intune API](https://docs.microsoft.com/intune/intune-graph-apis)。</span><span class="sxs-lookup"><span data-stu-id="ea93a-126">[Use Azure AD to access the Intune API](https://docs.microsoft.com/intune/intune-graph-apis).</span></span>
- <span data-ttu-id="ea93a-127">了解如何使用 [PowerShell Intune 示例](https://github.com/microsoftgraph/powershell-intune-samples)执行常见任务。</span><span class="sxs-lookup"><span data-stu-id="ea93a-127">See how to perform common tasks by using the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples).</span></span>
- <span data-ttu-id="ea93a-128">了解如何[使用 Intune REST API](https://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/resources/intune_graph_overview)。</span><span class="sxs-lookup"><span data-stu-id="ea93a-128">Find out how to [use the Intune REST API](https://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/resources/intune_graph_overview).</span></span>
- <span data-ttu-id="ea93a-129">有关 Intune API 中新增功能的信息，请参阅[更改日志](changelog.md)。</span><span class="sxs-lookup"><span data-stu-id="ea93a-129">See the [Changelog](changelog.md) for information about what's new in the Intune API.</span></span>
- <span data-ttu-id="ea93a-130">浏览[示例](https://developer.microsoft.com/zh-CN/graph/graph/examples)，了解有关如何使用 Microsoft Graph 的更多信息。</span><span class="sxs-lookup"><span data-stu-id="ea93a-130">Explore [examples](https://developer.microsoft.com/zh-CN/graph/graph/examples) for more ideas about how to use Microsoft Graph.</span></span>
